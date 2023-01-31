# Initiation Ansible

L'initiation d'Ansible par ligne de commande comprend les étapes suivantes :

1. Installation d'Ansible : Ansible peut être installé sur une machine Linux en utilisant le gestionnaire de paquets (apt ou yum) ou via pip pour Python.
2. Configuration de la cible : Définissez les cibles que vous souhaitez gérer dans un fichier appelé "inventory".
3. Écriture d'un playbook : Créez un fichier YAML contenant les tâches que vous souhaitez exécuter sur les cibles.
4. Exécution d'un playbook : Utilisez la commande "ansible-playbook" pour exécuter le playbook sur les cibles définies dans l'inventaire.

Exemple :

```yaml
# Installation d'Ansible
$ sudo apt-get install ansible

# Configuration de l'inventaire
$ nano /etc/ansible/hosts
[targets]
server1 ansible_host=192.168.1.100
server2 ansible_host=192.168.1.101

# Écriture d'un playbook
$ nano example.yml
---
- hosts: targets
  tasks:
  - name: Install Apache
    become: true
    apt: name=apache2 state=present

# Exécution d'un playbook
$ ansible-playbook example.yml
```

Ce sont les étapes de base pour démarrer avec Ansible en ligne de commande. Il existe de nombreuses autres fonctionnalités et options disponibles pour les playbooks, les tâches et les modules. Il est recommandé de consulter la documentation d'Ansible pour en savoir plus.
