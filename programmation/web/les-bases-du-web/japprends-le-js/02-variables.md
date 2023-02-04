# Javascript Variables

## Variables : Comment déclarer et affecter des valeurs à des variables en JavaScript.

Les variables en JavaScript permettent de stocker des valeurs telles que des nombres, des chaînes de caractères, des booléens, et des objets. Il est important de donner à une variable un nom significatif pour faciliter la lecture et la maintenance du code.

Pour déclarer une variable en JavaScript, vous utiliserez la syntaxe suivante :

```javascript
var nomDeVariable;
```

ou

```javascript
let nomDeVariable;
```

ou

```javascript
const nomDeVariable;
```

La différence entre **var**, **let** et **const** est que var est le plus ancien et peut être réaffecté après sa déclaration, let est similaire à var mais il ne peut pas être redéclaré dans la même portée, et const est similaire à let mais une fois qu'on lui assigne une valeur elle ne peut plus être modifiée.

Pour affecter une valeur à une variable, vous pouvez utiliser l'opérateur d'affectation (=) comme ceci :

```javascript
var nomDeVariable = valeur;
```

Par exemple :

```javascript
var age = 20;
let nom = "Alice";
const pi = 3.14;
```

Il est également possible de déclarer et affecter des valeurs à une variable en une seule ligne en utilisant la syntaxe suivante :

```javascript
let nomDeVariable = valeur;
```

Il est important de noter que les noms de variables en JavaScript sont sensibles à la casse, c'est-à-dire qu'une variable nommée "nomDeVariable" est différente d'une variable nommée "Nomdevariable". Il est donc important de respecter la casse lors de la déclaration et de l'utilisation des variables.

En résumé, les variables en JavaScript permettent de stocker des valeurs dans un programme. Il existe 3 types de déclaration de variable var, let et const qui ont des comportements différents. Pour déclarer une variable on utilise var, let ou const suivi d'un nom qui ne peut pas être un mot réservé et pour lui donner une valeur on utilise l'opérateur d'affectation (=) suivi de la valeur à affecter.
