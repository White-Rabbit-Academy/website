# Déploiement de clés SSH

Le déploiement de clés SSH permet de se connecter à des serveurs sans avoir à saisir un mot de passe à chaque fois. Voici les étapes à suivre pour l'automatisation de la configuration des clés SSH :

1. Générer une nouvelle paire de clés SSH en utilisant la commande "ssh-keygen".
2. Copier la clé publique sur le serveur distant avec la commande "ssh-copy-id \[user@]host".
3. Vérifier la connexion au serveur distant sans mot de passe en utilisant la commande "ssh \[user@]host".

Exemple :

```bash
# Génération de la paire de clés SSH
$ ssh-keygen

# Copie de la clé publique sur le serveur distant
$ ssh-copy-id user@host

# Connexion au serveur distant sans mot de passe
$ ssh user@host
```

Ces étapes peuvent également être automatisées en utilisant des scripts shell, des outils de configuration de système comme Ansible, Chef ou Puppet, ou en utilisant des services de gestion de clés tels que Hashicorp Vault.
