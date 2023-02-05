# Méthodes

Le point 5 clé de l'apprentissage de Java est la compréhension des méthodes. Les méthodes sont des blocs de code qui peuvent être réutilisés à plusieurs endroits dans une application. Les méthodes sont déclarées en utilisant la syntaxe suivante :

```java
<type de retour> nomDeLaMéthode(<liste d'arguments>) {
  // corps de la méthode
}
```

Par exemple, voici une méthode qui calcule la somme de deux entiers :

```java
int somme(int a, int b) {
  return a + b;
}
```

Dans cet exemple, la méthode s'appelle `somme`, prend deux arguments de type entier `a` et `b` et retourne un entier correspondant à la somme de `a` et `b`.

Les méthodes peuvent être appelées en utilisant leur nom suivi d'une liste d'arguments entre parenthèses, comme ceci :

```java
int resultat = somme(1, 2);
```

Dans ce cas, la méthode `somme` est appelée avec les arguments `1` et `2`, et le résultat de l'appel de la méthode est stocké dans la variable `resultat`.

Les méthodes peuvent être utilisées pour séparer le code en blocs logiques plus petits et plus faciles à comprendre, pour réduire la duplication de code et pour rendre le code plus maintenable. Il est important de comprendre comment déclarer et utiliser les méthodes en Java pour écrire du code plus efficace et plus lisible.
