# L’enchaînement de commandes

L'enchaînement de commandes dans un script bash implique l'exécution séquentielle de plusieurs commandes pour accomplir une tâche spécifique.

Voici un exemple simple de script bash qui utilise l'enchaînement de commandes :

```bash
#!/bin/bash

echo "Début du script."

# Déclaration de variables
nom="Alice Snow"
age=20

# Affichage des variables
echo "Bonjour, mon nom est $nom et j'ai $age ans."

# Exécution de la commande date pour afficher la date actuelle
date

# Boucle for pour afficher les nombres de 1 à 5
for i in {1..5}; do
  echo $i
done

echo "Fin du script."
```

Lorsque ce script est exécuté, il affichera le résultat suivant :

```
Début du script.
Bonjour, mon nom est Alice Snown et j'ai 20 ans.
Fri Jan 27 14:35:45 PST 2023
1
2
3
4
5
Fin du script.
```

Comme vous pouvez le voir, les différentes commandes sont exécutées les unes après les autres, avec un affichage de chaque commande. C'est ainsi que les scripts bash peuvent automatiser les tâches complexes en utilisant une séquence d'instructions simples.
