# Les instructions de base en pseudo-code

Le pseudo-code est un langage informel utilisé pour décrire un algorithme avant de le coder dans un langage de programmation formel. Les instructions de base en pseudo-code incluent :

1. Affectation : Attribuer une valeur à une variable. Par exemple : "nombre = 5".
2. Entrée : Lire une valeur saisie par l'utilisateur. Par exemple : "saisir nombre".
3. Sortie : Afficher une valeur ou un message à l'utilisateur. Par exemple : "afficher "Le nombre est : " + nombre".
4. Si (condition) : Exécuter un bloc d'instructions conditionnellement si une condition est remplie. Par exemple : "si nombre est supérieur à 10, afficher "Le nombre est grand".
5. Pour (boucle) : Répéter un bloc d'instructions plusieurs fois. Par exemple : "pour i de 1 à 10, afficher i".
6. Tant que (boucle) : Répéter un bloc d'instructions tant qu'une condition est remplie. Par exemple : "tant que nombre est inférieur à 100, augmenter nombre de 1".

Ces instructions de base peuvent être combinées pour créer des algorithmes plus complexes. Le pseudo-code est souple et peut varier selon les personnes ou les contextes, mais il a pour but de fournir une description claire et compréhensible de l'algorithme.

Voici un exemple de pseudo-code complet qui résout le problème de trouver le nombre le plus grand dans une liste d'entiers :

```
saisir nombre_de_nombres
déclarer tableau nombres[nombre_de_nombres]
déclarer plus_grand_nombre = 0

pour i de 0 à nombre_de_nombres - 1 faire
    saisir nombres[i]
    si nombres[i] > plus_grand_nombre alors
        plus_grand_nombre = nombres[i]
    fin_si
fin_pour

afficher "Le plus grand nombre est : " + plus_grand_nombre
```

Ce pseudo-code lit en premier le nombre de nombres dans la liste. Il déclare ensuite un tableau pour stocker ces nombres et une variable pour stocker le plus grand nombre trouvé. Ensuite, il utilise une boucle "pour" pour lire les nombres de la liste un par un, et utilise une structure conditionnelle "si" pour comparer chaque nombre avec le plus grand nombre trouvé jusqu'à présent. Finalement, il affiche le plus grand nombre trouvé.
