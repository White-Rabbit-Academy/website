# Classes et objets

Le point 6 clé de l'apprentissage de Java est la compréhension des classes et des objets. En Java, les classes sont des modèles pour les objets. Les objets sont des instances de classes et représentent des entités concrètes telles que des personnes, des voitures, etc.

Par exemple, une classe `Personne` peut définir les propriétés telles que le nom et l'âge d'une personne, ainsi que les méthodes pour obtenir et définir ces propriétés. Voici un exemple de classe `Personne` :

```java
class Personne {
  private String nom;
  private int age;

  public Personne(String nom, int age) {
    this.nom = nom;
    this.age = age;
  }

  public String getNom() {
    return nom;
  }

  public void setNom(String nom) {
    this.nom = nom;
  }

  public int getAge() {
    return age;
  }

  public void setAge(int age) {
    this.age = age;
  }
}
```

Dans cet exemple, la classe `Personne` définit les propriétés `nom` et `age`, ainsi que les méthodes `getNom`, `setNom`, `getAge` et `setAge` pour obtenir et définir ces propriétés.

Pour utiliser cette classe, nous pouvons créer des objets `Personne` en utilisant le mot-clé `new`, comme ceci :

```java
Personne p1 = new Personne("John Doe", 30);
Personne p2 = new Personne("Jane Doe", 25);
```

Dans ce cas, nous créons deux objets `Personne`, `p1` et `p2`, en utilisant la classe `Personne`. Nous pouvons ensuite accéder aux propriétés et aux méthodes de ces objets en utilisant le point `.`, comme ceci :

```java
System.out.println(p1.getNom() + " is " + p1.getAge() + " years old.");
System.out.println(p2.getNom() + " is " + p2.getAge() + " years old.");
```

La compréhension des classes et des objets est un aspect important de la programmation orientée objet en Java, et il est important de comprendre comment déclarer et utiliser des classes et des objets pour écrire du code plus efficace et plus lisible.
