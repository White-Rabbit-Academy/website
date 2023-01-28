# Gestion des utilisateurs, des groupes et des mots de passe

La gestion des utilisateurs, des groupes et des mots de passe sous Linux permet de créer et gérer les comptes utilisateur, les groupes d'utilisateurs et les mots de passe associés.

Voici quelques commandes courantes pour gérer les utilisateurs, les groupes et les mots de passe sous Linux :

* Pour créer un utilisateur : "`useradd nom_utilisateur`"
* Pour supprimer un utilisateur : "`userdel nom_utilisateur`"
* Pour modifier les informations d'un utilisateur : "`usermod nom_utilisateur`"
* Pour lister les utilisateurs : "`cat /etc/passwd`"
* Pour créer un groupe : "`groupadd nom_groupe`"
* Pour supprimer un groupe : "`groupdel nom_groupe`"
* Pour ajouter un utilisateur à un groupe : "`usermod -a -G nom_groupe nom_utilisateur`"
* Pour lister les groupes : "`cat /etc/group`"
* Pour changer un mot de passe utilisateur : "`passwd nom_utilisateur`"
* Pour forcer un utilisateur à changer son mot de passe lors de sa prochaine connexion : "`passwd -e nom_utilisateur`"
* Pour verifier si un mot de passe est valide : "`passwd -S nom_utilisateur`"

Voici quelques exemples d'utilisation de ces commandes :

* Pour créer un utilisateur nommé "johndoe" avec le groupe "users" et un répertoire personnel :

```bash
useradd -m -g users johndoe
```

* Pour ajouter l'utilisateur "johndoe" au groupe "sudo" :

```bash
usermod -a -G sudo johndoe
```

* Pour forcer l'utilisateur "johndoe" à changer son mot de passe lors de sa prochaine connexion :

```bash
passwd -e johndoe
```

Il est important de noter que ces commandes et les options disponibles peuvent varier en fonction de la distribution Linux utilisée. Il est donc recommandé de se référer à la documentation de la distribution pour connaître les commandes exactes à utiliser.

Il est également important de noter que les utilisateurs et les groupes créés doivent être correctement configurés pour les permissions d'accès aux fichiers et aux répertoires, cela peut être fait avec les commandes chmod, chown, setfacl etc.
