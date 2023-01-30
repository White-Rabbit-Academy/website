# Les conditions et les tests

Les conditions et les tests en bash permettent de prendre des décisions dans un script en fonction des résultats d'un test. Les tests peuvent être de différents types, tels que les tests de comparaison de nombres, les tests de comparaison de chaînes, les tests de fichiers, etc.

Voici un exemple simple de script bash qui utilise des conditions et des tests :

```bash
#!/bin/bash

echo "Entrez un nombre :"
read nombre

# Test de comparaison de nombres
if [ $nombre -lt 10 ]; then
  echo "Le nombre est inférieur à 10."
else
  echo "Le nombre est supérieur ou égal à 10."
fi
```

Lorsque ce script est exécuté, il demandera à l'utilisateur d'entrer un nombre, puis effectuera un test pour vérifier si ce nombre est inférieur à 10. En fonction du résultat de ce test, le script affichera l'une des deux phrases suivantes :

* "Le nombre est inférieur à 10."
* "Le nombre est supérieur ou égal à 10."

Les conditions et les tests sont un élément clé de la programmation de scripts bash et peuvent être utilisés pour créer des scripts plus complexes et plus flexibles.

## En détail

Le constructeur `if` en bash permet de tester une condition et d'exécuter un bloc de commandes spécifique en fonction du résultat du test. La syntaxe générale du constructeur `if` est la suivante :

```bash
if [ condition ]; then
  # commandes à exécuter si la condition est vraie
else
  # commandes à exécuter si la condition est fausse
fi
```

Les types de conditions disponibles en bash incluent :

1. Test de comparaison de nombres : utilisez les opérateurs de comparaison numériques (`-lt` pour "inférieur à", `-gt` pour "supérieur à", etc.) pour comparer deux nombres.

```bash
# Exemple
if [ $nombre1 -lt $nombre2 ]; then
  echo "nombre1 est plus petit que nombre2."
fi
```

2. Test de comparaison de chaînes : utilisez les opérateurs de comparaison de chaînes (`=` pour "égal à", `!=` pour "différent de", etc.) pour comparer deux chaînes.

```bash
# Exemple
if [ "$nom" = "John Doe" ]; then
  echo "Le nom est John Doe."
fi
```

3. Test de fichiers : utilisez les opérateurs de test de fichiers (`-e` pour "existe", `-f` pour "est un fichier", etc.) pour vérifier l'existence et les propriétés d'un fichier.

```bash
# Exemple
if [ -e "/chemin/du/fichier" ]; then
  echo "Le fichier existe."
fi
```

4. Test de variables : utilisez les opérateurs de test de variables (`-z` pour "est vide", `-n` pour "n'est pas vide", etc.) pour vérifier les propriétés d'une variable.

```bash
# Exemple
if [ -z "$variable" ]; then
  echo "La variable est vide."
fi
```

Ces sont les types de conditions les plus couramment utilisés en bash, mais il existe d'autres opérateurs de test et de comparaison disponibles pour des tests plus avancés. Il est important de noter que toutes les conditions doivent être entourées de crochets (\[ ]) pour être valides en bash.
