# Javascript Conditions

## Conditions : Comment utiliser des instructions if-else et switch pour créer des conditions dans votre code.

Les instructions de condition en JavaScript vous permettent de vérifier si une condition est vraie ou fausse, et d'exécuter un certain code en conséquence. Les instructions if-else et switch sont les deux principales structures de contrôle de flux utilisées pour créer des conditions en JavaScript.

L'instruction if-else est utilisée pour vérifier si une condition est vraie, et exécuter un certain code si c'est le cas. Elle a la syntaxe suivante :

```javascript
if (condition) {
    // code à exécuter si la condition est vraie
} else {
    // code à exécuter si la condition est fausse
}
```

Voici un exemple d'utilisation de l'instruction if-else :

```javascript
let age = 25;
let ageMinimum = 18;

if (age >= ageMinimum) {
    console.log("Vous êtes majeur");
} else {
    console.log("Vous n'êtes pas majeur");
}

```

L'instruction switch est utilisée pour vérifier si une valeur correspond à une des options définies. Il a la syntaxe suivante :

```javascript
switch (expression) {
    case valeur1:
        // code à exécuter si expression est égale à valeur1
        break;
    case valeur2:
        // code à exécuter si expression est égale à valeur2
        break;
    // ...
    default:
        // code à exécuter si expression ne correspond à aucune des valeurs
}
```

Voici un exemple d'utilisation de l'instruction switch :

```javascript
let jour = "lundi";

switch (jour) {
    case "lundi":
        console.log("Premier jour de la semaine");
        break;
    case "mardi":
        console.log("Deuxième jour de la semaine");
        break;
    // ...
    default:
        console.log("Jour non reconnu");
}

```

Il est important de noter que dans l'instruction switch, chaque instruction doit être suivie d'un _**break**_ pour indiquer la fin de l'instruction, sauf pour la dernière instruction qui peut être omis.

En résumé, les instructions if-else et switch sont utilisées pour créer des conditions en JavaScript. L'instruction if-else vérifie si une condition est vraie ou fausse, et exécute un certain code en conséquence. L'instruction switch vérifie si une valeur correspond à une des options définies et exécute le code correspondant. Ces instructions permettent de définir des chemins d'exécution différents en fonction des conditions et des valeurs données.
