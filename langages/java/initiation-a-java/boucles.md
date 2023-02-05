# Boucles

Le point 3 clé de l'apprentissage de Java est la compréhension des boucles. Les boucles permettent de répéter un bloc de code plusieurs fois en fonction d'une condition spécifiée. Il existe deux types de boucles en Java : les boucles for et les boucles while.

* Les boucles for :

```java
for (int i = 0; i < 10; i++) {
  System.out.println("Ligne " + i);
}
```

Dans cet exemple, la boucle for s'exécutera 10 fois. La variable `i` est initialisée à 0, la condition `i < 10` est vérifiée avant chaque itération de la boucle et `i++` est exécuté après chaque itération de la boucle pour incrémenter la valeur de `i`.

* Les boucles while :

```java
int i = 0;
while (i < 10) {
  System.out.println("Ligne " + i);
  i++;
}
```

Dans cet exemple, la boucle while s'exécutera 10 fois également. La variable `i` est initialisée à 0 et la condition `i < 10` est vérifiée avant chaque itération de la boucle. La valeur de `i` est incrémentée à l'intérieur de la boucle.

L'utilisation des boucles est essentielle pour effectuer des tâches répétitives en Java, telles que le parcours de tableaux ou la génération de nombres aléatoires. Il est important de comprendre comment fonctionnent les boucles et comment les utiliser correctement pour écrire du code qui fonctionne correctement et de manière efficace.
