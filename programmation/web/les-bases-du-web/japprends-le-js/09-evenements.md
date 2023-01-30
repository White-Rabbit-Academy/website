# Javascript Événements

## Événements : Comment utiliser les événements pour créer des interactions utilisateur en JavaScript.

Les événements en JavaScript permettent de réagir aux actions de l'utilisateur sur une page web, comme un clic de souris, une saisie de texte, une modification de la page, etc. Pour utiliser les événements, il faut d'abord sélectionner l'élément sur lequel l'événement doit être déclenché, puis utiliser la méthode addEventListener pour ajouter un gestionnaire d'événement à cet élément.

Par exemple, pour réagir à un clic de souris sur un bouton :

```javascript
let bouton = document.getElementById("monBouton");
bouton.addEventListener("click", function() {
    console.log("Bouton cliqué!");
});
```

Il existe de nombreux types d'événements différents qui peuvent être utilisés, comme `"click"`, `"mouseover"`, `"submit"`, `"keydown"`, etc. Il est important de noter que plusieurs gestionnaires d'événements peuvent être ajoutés à un même élément pour réagir à différents types d'événements.

Il est également possible de supprimer un événement en utilisant la méthode `removeEventListener`. Il suffit de fournir le type d'événement et la fonction de gestionnaire d'événements à supprimer.

En résumé, les événements en JavaScript permettent de réagir aux actions de l'utilisateur sur une page web. Pour utiliser les événements, il faut sélectionner l'élément sur lequel l'événement doit être déclenché et utiliser la méthode `addEventListener` pour ajouter un gestionnaire d'événement à cet élément. Il existe de nombreux types d'événements différents qui peuvent être utilisés, et il est possible de supprimer un événement en utilisant la méthode `removeEventListener`.
