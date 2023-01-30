# Les fonctions

Les fonctions en bash permettent de regrouper un ensemble de commandes en un seul bloc, ce qui permet de les exécuter plusieurs fois avec des paramètres différents. La syntaxe générale pour définir une fonction est la suivante :

```python
nom_fonction () {
  # commandes à exécuter pour la fonction
}
```

Exemple :

```bash
# Définition d'une fonction qui affiche le double d'un nombre
double () {
  resultat=$(( $1 * 2 ))
  echo "Le double de $1 est $resultat"
}

# Appel de la fonction avec le nombre 5
double 5
```

Les fonctions peuvent également prendre plusieurs paramètres en plus d'un seul :

```bash
# Définition d'une fonction qui calcule la somme de deux nombres
somme () {
  resultat=$(( $1 + $2 ))
  echo "La somme de $1 et $2 est $resultat"
}

# Appel de la fonction avec les nombres 3 et 5
somme 3 5
```

Il est important de noter que les fonctions en bash ne retournent pas de valeur comme en d'autres langages de programmation, mais elles peuvent utiliser la variable de sortie standard (stdout) pour retourner des valeurs à l'appelant.
