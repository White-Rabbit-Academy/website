# Les mécanismes de boucles

En bash, il existe plusieurs mécanismes de boucle pour exécuter un bloc de commandes plusieurs fois. Voici les types de boucles les plus couramment utilisés :

1. Boucle `for` : la boucle `for` permet d'itérer sur une liste d'éléments, tels que des mots ou des nombres. La syntaxe générale est la suivante :

```bash
for variable in liste; do
  # commandes à exécuter pour chaque élément de la liste
done
```

Exemple :

```bash
# Boucle for sur une liste de mots
for mot in un deux trois; do
  echo $mot
done

# Boucle for sur une plage de nombres
for (( i=1; i<=5; i++ )); do
  echo $i
done
```

2. Boucle `while` : la boucle `while` permet d'exécuter un bloc de commandes tant que la condition spécifiée est vraie. La syntaxe générale est la suivante :

```bash
while [ condition ]; do
  # commandes à exécuter tant que la condition est vraie
done
```

Exemple :

```bash
# Boucle while pour afficher les nombres de 1 à 5
i=1
while [ $i -le 5 ]; do
  echo $i
  i=$(( i + 1 ))
done
```

3. Boucle `until` : la boucle `until` est similaire à la boucle `while`, mais s'exécute tant que la condition spécifiée est fausse. La syntaxe générale est la suivante :

```bash
until [ condition ]; do
  # commandes à exécuter tant que la condition est fausse
done
```

Exemple :

```bash
# Boucle until pour afficher les nombres de 1 à 5
i=6
until [ $i -le 5 ]; do
  echo $i
  i=$(( i - 1 ))
done
```

Ces sont les trois types de boucles les plus couramment utilisés en bash, mais il existe d'autres mécanismes de boucle tels que la boucle `select` pour des cas d'utilisation plus avancés. Il est important de noter que les instructions de boucle doivent être entourées de mots clés tels que `do` et `done` pour être valides en bash.
