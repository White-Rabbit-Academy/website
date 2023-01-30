# Javascript DOM

## DOM : Comment accéder et manipuler des éléments HTML à l'aide de JavaScript.

Le Document Object Model (DOM) est une interface de programmation pour les documents HTML et XML, qui permet de manipuler les éléments de la page en utilisant JavaScript. Il permet de sélectionner, créer, modifier et supprimer des éléments HTML, ainsi que d'accéder aux propriétés et aux attributs de ces éléments.

Pour sélectionner des éléments HTML, on peut utiliser les méthodes `getElementById`, `getElementsByTagName` et `getElementsByClassName`. Par exemple :

```javascript
let titre = document.getElementById("titre");
let paragraphes = document.getElementsByTagName("p");
let rouge = document.getElementsByClassName("rouge");
```

Pour créer des éléments HTML, on peut utiliser la méthode `createElement` et ajouter des propriétés et des attributs à ces éléments en utilisant les propriétés `innerHTML`, `setAttribute`, etc. Par exemple :

```javascript
let nouveauParagraphe = document.createElement("p");
nouveauParagraphe.innerHTML = "Ceci est un nouveau paragraphe";
nouveauParagraphe.setAttribute("class", "rouge");
document.body.appendChild(nouveauParagraphe);
```

Pour modifier des éléments HTML, on peut utiliser les propriétés `innerHTML` et `value`, ainsi que les méthodes **setAttribute** et **classList.add/remove/toggle**. Par exemple :

```javascript
titre.innerHTML = "Nouveau titre";
bouton.value = "Cliquez ici";
bouton.setAttribute("disabled", true);
bouton.classList.add("rouge");
```

Pour supprimer des éléments HTML, on peut utiliser la méthode `removeChild` ou `remove` . Par exemple :

```javascript
document.body.removeChild(nouveauParagraphe);
nouveauParagraphe.remove();
```

En résumé, le Document Object Model (DOM) est une interface de programmation pour les documents HTML et XML qui permet de manipuler les éléments de la page en utilisant JavaScript. Il permet de sélectionner, créer, modifier et supprimer des éléments HTML, ainsi que d'accéder aux propriétés et aux attributs de ces éléments. Les méthodes comme `getElementById`, `createElement`, `appendChild`, `innerHTML`, `setAttribute`, etc sont utilisées pour les différentes opérations.
