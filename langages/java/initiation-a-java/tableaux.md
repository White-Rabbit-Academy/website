# Tableaux

Le point 4 clé de l'apprentissage de Java est la compréhension des tableaux. Les tableaux sont des structures de données qui permettent de stocker plusieurs valeurs du même type dans un seul objet. Les tableaux sont déclarés en utilisant le type de données suivi d'une paire de crochets. Par exemple :

```java
int[] monTableau = new int[5];
```

Dans cet exemple, nous déclarons un tableau d'entiers appelé `monTableau` qui peut stocker jusqu'à 5 valeurs. Les valeurs peuvent être accédées en utilisant un index compris entre 0 et 4, par exemple `monTableau[0]` pour accéder à la première valeur du tableau.

Il est également possible de déclarer et initialiser un tableau en même temps :

```java
int[] monTableau = {1, 2, 3, 4, 5};
```

Dans cet exemple, nous déclarons un tableau d'entiers avec les valeurs initiales `1, 2, 3, 4, 5`.

Les tableaux sont souvent utilisés pour stocker des collections de données et peuvent être parcourus à l'aide de boucles pour effectuer des opérations sur chaque élément. Par exemple, pour imprimer chaque valeur du tableau `monTableau` :

```java
for (int i = 0; i < monTableau.length; i++) {
  System.out.println(monTableau[i]);
}
```

Il est important de comprendre comment déclarer, initialiser et utiliser les tableaux pour écrire du code plus efficace et maintenable en Java.
