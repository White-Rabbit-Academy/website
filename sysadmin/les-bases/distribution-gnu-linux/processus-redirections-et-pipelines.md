# Processus, redirections et pipelines

Les processus sous Linux sont des programmes en cours d'exécution. Chaque processus a un numéro d'identification unique (PID) qui peut être utilisé pour effectuer des actions sur ce processus, comme le tuer ou le suspendre.

Les redirections et les pipelines sont des mécanismes utilisés pour connecter les sorties et les entrées des processus entre eux.

La redirection permet de rediriger la sortie standard d'un processus vers un fichier ou vers l'entrée standard d'un autre processus. Les opérateurs de redirection les plus couramment utilisés sont :

* `>` pour rediriger la sortie standard vers un fichier (remplace le contenu du fichier s'il existe déjà)
* `>>` pour ajouter la sortie standard à un fichier (ajoute au contenu existant s'il existe déjà)
* `<` pour rediriger l'entrée standard à partir d'un fichier

Les pipelines permettent de connecter la sortie standard d'un processus à l'entrée standard d'un autre processus en utilisant le symbole `|`. Cela permet de chaîner des commandes ensemble pour créer des commandes plus puissantes.

Voici un exemple de l'utilisation de la redirection et des pipelines :

```bash
ls -l /usr/bin/ | grep python > python_commands.txt
```

Cette commande utilise d'abord la commande `ls -l /usr/bin/` pour lister les fichiers dans le répertoire /usr/bin/ et redirige sa sortie standard vers la commande `grep python` qui recherche les lignes contenant "python" dans la sortie de la commande précédente. Enfin, la sortie de `grep` est redirigée vers le fichier "python\_commands.txt".

Il est important de noter que l'ordre des commandes dans les pipelines et les redirections est important car cela détermine l'ordre dans lequel les données sont traitées par chaque commande.
