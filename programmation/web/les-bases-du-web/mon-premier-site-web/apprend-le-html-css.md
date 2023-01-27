---
cover: ../../../../.gitbook/assets/pexels-designecologist-1779487.jpg
coverY: 73
---

# Apprend le html css

## Les débuts dans le WEB

HTML (Hypertext Markup Language) et CSS (Cascading Style Sheets) sont des langages de programmation utilisés pour créer des pages web.

HTML est utilisé pour structurer le contenu d'une page web. Il permet de créer des titres, des paragraphes, des images, des liens, etc. Les balises HTML sont utilisées pour indiquer le type de contenu à afficher, par exemple

pour un paragraphe ou  pour une image.

CSS est utilisé pour styliser le contenu créé avec HTML. Il permet de changer la couleur, la taille, la police, la disposition, etc. des éléments HTML. Les règles CSS sont appliquées aux éléments HTML en utilisant des sélecteurs, comme par exemple #monid pour un élément avec l'attribut `id="monid"` ou `.maClasse` pour tous les éléments avec la classe "**maClasse**".

Voici un exemple de base d'une page web créée avec HTML et CSS :

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Ma page web</title>
    <style>
      /* Règles CSS */
      h1 {
        color: blue;
      }
    </style>
  </head>
  <body>
    <h1>Titre de ma page</h1>
    <p>Contenu de ma page</p>
  </body>
</html>
```

Ce code crée une page web avec un titre de niveau 1 (balise `<h1>`) affiché en bleu et un paragraphe (balise `<p>`) avec du contenu.

> Il y a beaucoup plus à apprendre sur HTML et CSS, il existe de nombreux cours et tutoriels en ligne pour vous aider à en apprendre davantage. Je vous recommande de consulter des sites tels que [W3Schools](https://www.w3schools.com/html/html\_exercises.asp) ou [MDN Web Docs](https://developer.mozilla.org/fr/) pour des informations détaillées et des exercices pratiques.

#### Les bases du HTML

Pour continuer, voici quelques éléments HTML couramment utilisés :

* Les titres : les balises `<h1>` à `<h6>` sont utilisées pour les titres de différents niveaux.
* Les paragraphes : la balise `<p>` est utilisée pour les paragraphes de texte.
* Les images : la balise `<img>` est utilisée pour afficher des images. Elle prend des attributs tels que src (source de l'image) et alt (texte alternatif pour les utilisateurs qui ne peuvent pas voir l'image).
* Les liens : la balise `<a>` est utilisée pour créer des liens. L'attribut href contient l'URL de la page vers laquelle le lien pointe.
* Les listes : les balises `<ul>` (liste à puces) et `<ol>` (liste numérotée) sont utilisées pour créer des listes. Les balises `<li>` sont utilisées pour chaque élément de la liste.

#### Les bases du CSS

En ce qui concerne CSS, voici quelques propriétés couramment utilisées :

* La propriété `color` permet de changer la couleur du texte.
* La propriété `background-color` permet de changer la couleur de fond d'un élément.
* La propriété `font-size` permet de changer la taille de la police.
* La propriété `text-align` permet d'aligner le texte (à gauche, au centre, à droite).
* La propriété `margin` et `padding` permet de définir des marges et des espacements autour d'un élément.
* La propriété `display` permet de définir comment un élément est affiché (en ligne, en bloc, en table, etc.).

### Un petit exo ?

Voici un exercice pour vous aider à créer votre première page web en utilisant HTML et CSS :

1. Ouvrez un éditeur de code (comme Sublime Text, Notepad++ ou Visual Studio Code) et créez un nouveau fichier.
2. Ajoutez les balises de base d'une page HTML en utilisant la structure suivante :

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Ma première page web</title>
  </head>
  <body>
  </body>
</html>
```

Dans la section `<body>`, ajoutez un titre de niveau 1 en utilisant la balise `<h1>`. Par exemple :

```html
<h1>Bienvenue sur ma première page web</h1>
```

Ajoutez un paragraphe de texte en utilisant la balise `<p>`. Par exemple :

```html
<p>Je suis en train d'apprendre à créer des pages web en utilisant HTML et CSS.</p>
```

Ajoutez une image en utilisant la balise `<img>`. Assurez-vous d'utiliser un lien valide pour l'attribut src de l'image. Par exemple :

```html
<img src="https://images.unsplash.com/photo-1524726240783-939bfdd633e2?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1974&q=80" alt="Une photo de paysage">
```

Ajoutez un lien en utilisant la balise `<a>` Assurez-vous d'utiliser un lien valide pour l'attribut **href** du lien. Par exemple :

```html
<a href="https://fr.wikipedia.org/wiki/Tortue">En savoir plus sur les tortues</a>
```

Dans la section `<head>`, ajoutez une balise `<style>` pour inclure des règles CSS. Par exemple :

```html
<style>
  /* Règles CSS */
  body {
    background-color: #f0f0f0;
  }
  h1 {
    color: blue;
    text-align: center;
  }
</style>
```

Enregistrez le fichier avec l'extension .html (par exemple, "ma\_premiere\_page.html") et ouvrez-le dans un navigateur web pour voir votre page.

Ce n'est qu'un exemple simple pour vous aider à comprendre les bases de la création d'une page web en utilisant HTML et CSS. Vous pouvez continuer à ajouter des éléments et à expérimenter avec des propriétés CSS pour personnaliser votre page. N'oubliez pas de consulter les références en ligne pour obtenir de l'aide et des exemples de code.

Il existe également des frameworks CSS tels que Bootstrap ou Foundation qui peuvent vous faciliter la création d'une page web en fournissant des classes prédéfinies pour les éléments courants (comme les boutons, les formulaires, les grilles, etc.). Ces frameworks peuvent vous éviter de devoir écrire beaucoup de CSS de base et vous permettre de vous concentrer sur la conception de votre page.

Il est par ailleurs important de valider votre code pour vous assurer qu'il est conforme aux standards et qu'il fonctionne correctement sur différents navigateurs. Il existe des outils en ligne tels que le validateur HTML de W3C ou le débogueur de code de Chrome qui peuvent vous aider à repérer les erreurs dans votre code.

En résumé, créer une page web en utilisant HTML et CSS est un processus qui nécessite une compréhension des balises et des propriétés couramment utilisées, ainsi qu'une pratique et de la patience. Il existe de nombreuses ressources en ligne pour vous aider à apprendre et à perfectionner vos compétences.
