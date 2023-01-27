# 05 - Boucles

## Boucles : Comment utiliser les boucles for et while pour répéter des actions dans votre code.

Les boucles en JavaScript permettent de répéter des actions plusieurs fois, ce qui est utile pour traiter des données en série ou pour créer des animations. Il existe deux principaux types de boucles en JavaScript : les boucles for et les boucles while.

La boucle for est utilisée pour exécuter une série d'instructions un nombre défini de fois. Elle a la syntaxe suivante :

```javascript
for (initialisation; condition; incrémentation) {
    // code à exécuter
}
```

Voici un exemple d'utilisation de la boucle for :

```javascript
for (let i = 0; i < 10; i++) {
    console.log(i);
}
```

La boucle while est utilisée pour exécuter une série d'instructions tant que la condition est vraie. Elle a la syntaxe suivante :

```javascript
let i = 0;
while (i < 10) {
    console.log(i);
    i++;
}
```

Il est important de noter que si la condition de la boucle while n'est jamais vraie, le code à l'intérieur de la boucle ne sera jamais exécuté, ce qui peut causer des problèmes de boucle infinie. Il est donc important de vérifier que la condition est correctement écrite pour éviter ce genre de problème.

Il existe aussi la boucle _**do-while**_ qui a la même syntaxe que while mais qui execute une première fois le code avant de vérifier la condition.

En résumé, les boucles for et while en JavaScript permettent de répéter des actions plusieurs fois. La boucle for est utilisée pour exécuter une série d'instructions un nombre défini de fois, tandis que la boucle while est utilisée pour exécuter une série d'instructions tant que la condition est vraie. Il est important de vérifier la condition pour éviter les problèmes de boucle infinie.
