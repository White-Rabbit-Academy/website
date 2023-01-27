# 06 - Fonctions

## Fonctions : Comment déclarer et utiliser des fonctions en JavaScript.

Les fonctions en JavaScript permettent de regrouper des instructions pour les exécuter à plusieurs endroits dans un programme. Les fonctions sont déclarées en utilisant la syntaxe _**function**_ suivie d'un nom de fonction et d'un ensemble de parenthèses qui peuvent contenir des paramètres. Par exemple :

```javascript
function nomDeFonction(parametre1, parametre2) {
    // instructions
}
```

On peut également utiliser une fonction fléchée qui est une syntaxe alternative pour déclarer une fonction, elle a la syntaxe suivante :

```javascript
const nomDeFonction = (parametre1, parametre2) => {
    // instructions
}
```

Une fois déclarée, une fonction peut être appelée ou invoquée en utilisant son nom suivi de parenthèses. Par exemple :

```javascript
nomDeFonction(arg1, arg2);
```

Les paramètres sont des variables qui sont utilisées pour passer des valeurs à une fonction lors de son appel. Les arguments sont les valeurs réelles qui sont passées à une fonction lors de son appel. Par exemple, dans l'exemple ci-dessus, **arg1** et **arg2** sont des arguments qui sont passés à la fonction _nomDeFonction_, qui utilise les paramètres **parametre1** et **parametre2** pour traiter ces valeurs.

Une fonction peut également retourner une valeur en utilisant l'instruction return. Par exemple :

```javascript
function addition(a, b) {
    return a + b;
}

let resultat = addition(3, 4); // resultat vaut 7
```

Les fonctions peuvent également être utilisées comme des variables, comme des paramètres pour d'autres fonctions ou comme valeurs de retour. Les fonctions anonymes sont des fonctions qui n'ont pas de nom et sont souvent utilisées en tant que paramètres pour d'autres fonctions.

En résumé, les fonctions en JavaScript permettent de regrouper des instructions pour les exécuter à plusieurs endroits dans un programme. Elles sont déclarées en utilisant la syntaxe _function_ suivie d'un nom de fonction et d'un ensemble de parenthèses qui peuvent contenir des paramètres. Une fois déclarée, une fonction peut être appelée ou invoquée en utilisant son nom suivi de parenthèses et en passant des arguments pour les paramètres. Les fonctions peuvent également retourner une valeur en utilisant l'instruction return. Les fonctions peuvent également être utilisées comme des variables, des paramètres pour d'autres fonctions ou des valeurs de retour. Les fonctions anonymes sont des fonctions qui n'ont pas de nom et sont souvent utilisées en tant que paramètres pour d'autres fonctions.
