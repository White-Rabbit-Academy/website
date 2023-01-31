# Playbooks et rôles Ansible

Les playbooks et les rôles Ansible sont des outils importants pour la gestion de configuration avec Ansible.

1. Playbooks Ansible : Les playbooks sont des scripts YAML qui décrivent les tâches à exécuter sur les cibles définies dans l'inventaire d'Ansible. Les playbooks peuvent être utilisés pour automatiser les tâches telles que l'installation de logiciels, la configuration de services, la définition des utilisateurs et des permissions, etc.
2. Rôles Ansible : Les rôles sont une façon d'organiser et de structurer les playbooks Ansible en encapsulant des tâches spécifiques pour un but particulier. Les rôles peuvent être partagés et réutilisés facilement entre plusieurs playbooks, ce qui facilite la gestion et la maintenance des tâches.

Voici comment mettre en place des playbooks et des rôles Ansible :

1. Créez un répertoire pour votre projet Ansible.
2. Créez un répertoire pour vos rôles à l'intérieur du projet.
3. Créez un playbook Ansible à l'intérieur du répertoire de projet.
4. Dans le playbook, spécifiez les rôles à utiliser en utilisant la directive "roles:" suivie des noms des rôles.
5. Exécutez le playbook en utilisant la commande "ansible-playbook".

Exemple :

```shell
# Création du répertoire de projet
$ mkdir myproject
$ cd myproject

# Création du répertoire de rôles
$ mkdir roles

# Création du playbook
$ nano main.yml
---
- hosts: all
  roles:
    - role1
    - role2

# Exécution du playbook
$ ansible-playbook main.yml
```

En utilisant les playbooks et les rôles Ansible, vous pouvez facilement organiser et automatiser les tâches de configuration sur vos cibles. Cela vous aide à gérer de manière efficace vos projets de configuration, à les maintenir et à les partager avec d'autres développeurs.
