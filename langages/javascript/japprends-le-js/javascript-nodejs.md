# Javascript Nodejs

Node.js est un environnement d'exécution JavaScript côté serveur. Il permet de développer des applications web en utilisant JavaScript sur le serveur plutôt que dans le navigateur.

Pour l'installer, vous pouvez télécharger le fichier d'installation depuis le site web de Node.js et l'exécuter sur votre ordinateur. Vous pouvez également utiliser un gestionnaire de paquets comme Homebrew pour macOS ou apt pour Linux pour l'installer.

Les grands principes de Node.js incluent :

* Utilisation de JavaScript sur le serveur
* Modèles d'exécution asynchrones et non bloquants pour améliorer les performances
* Utilisation d'une bibliothèque de modules pour partager du code et réutiliser des fonctionnalités
* Architecture orientée événements pour gérer les connexions réseau et les entrées/sorties de manière efficace.

### Les packages

Les packages sont des collections de modules et de fonctionnalités qui peuvent être partagés et réutilisés dans différentes applications Node.js. Ils sont gérés via le gestionnaire de paquets npm (Node Package Manager), qui est inclus avec Node.js.

Pour utiliser un package, vous devez d'abord l'installer dans votre projet en utilisant la commande npm :

```javascript
npm install nom-du-package
```

Une fois installé, vous pouvez l'utiliser dans votre code en utilisant require :

```javascript
var package = require('nom-du-package');
```

Il existe des milliers de packages disponibles sur npm, allant des bibliothèques de base de données aux bibliothèques de visualisation de données en passant par les bibliothèques pour les tests et les déploiements. En utilisant des packages, vous pouvez économiser du temps et de l'effort en réutilisant du code déjà écrit et testé, ainsi qu'en profitant des contributions de la communauté Node.js.
