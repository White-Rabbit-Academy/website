# L’utilisation de commandes internes / externes

En bash, il existe deux types de commandes : les commandes internes et les commandes externes.

Les commandes internes sont des fonctionnalités intégrées à la shell bash elle-même. Elles peuvent être utilisées sans avoir à charger un programme externe. Exemples de commandes internes : `cd`, `echo`, `pwd`, `read`, etc.

Les commandes externes, en revanche, sont des programmes externes qui sont appelés par la shell bash. Pour utiliser ces commandes, le programme externe doit être installé sur le système et accessible à partir du chemin d'accès. Exemples de commandes externes : `ls`, `grep`, `awk`, etc.

Voici un exemple de script bash qui utilise une commande interne (`echo`) et une commande externe (`ls`) :

```bash
#!/bin/bash

echo "Début du script."

# Utilisation de la commande interne echo
echo "Voici le contenu du répertoire actuel :"

# Utilisation de la commande externe ls
ls

echo "Fin du script."
```

Lorsque ce script est exécuté, il affichera le contenu du répertoire actuel, ce qui peut être différent d'un système à l'autre.
