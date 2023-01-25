# 07 - Tableaux et objets

## Tableaux et objets : Comment utiliser les tableaux et les objets pour stocker et manipuler des données en JavaScript.

Les tableaux et les objets en JavaScript sont des structures de données utilisées pour stocker et manipuler des données. Les tableaux sont utilisés pour stocker une série d'éléments de même type, tandis que les objets sont utilisés pour stocker des paires clé-valeur.

Les tableaux sont déclarés en utilisant la syntaxe `[]`, et les éléments sont séparés par une virgule. Par exemple :

```javascript
let fruits = ["pomme", "banane", "orange"];
```

Les éléments d'un tableau peuvent être accédés en utilisant leur index, qui est leur position dans le tableau. Les indexes sont des entiers commençant à 0 pour le premier élément, 1 pour le deuxième, etc. Par exemple :

```javascript
console.log(fruits[0]); // affiche "pomme"
```

Les objets sont déclarés en utilisant la syntaxe `{}`, et les propriétés sont définies en utilisant la syntaxe `nomDePropriété: valeur`. Par exemple :

```javascript
let personne = {
    nom: "Alice",
    age: 20,
    ville: "Luxembourg"
};
```

Les propriétés d'un objet peuvent être accédées en utilisant la notation point ou la notation crochet. Par exemple :

```javascript
console.log(personne.nom); // affiche "John"
console.log(personne["nom"]); // affiche "John"
```

Il est important de noter que les objets sont des structures de données non-ordonnées, contrairement aux tableaux qui sont ordonnés.

En résumé, les tableaux et les objets en JavaScript sont des structures de données utilisées pour stocker et manipuler des données. Les tableaux sont utilisés pour stocker une série d'éléments de même type, et les objets sont utilisés pour stocker des paires clé-valeur. Les éléments de tableaux peuvent être accédés en utilisant leur index, et les propriétés d'objets peuvent être accédées en utilisant la notation point ou la notation crochet. Les objets sont des structures de données non-ordonnées, contrairement aux tableaux qui sont ordonnés.
