---
cover: >-
  https://images.unsplash.com/photo-1604134967494-8a9ed3adea0d?crop=entropy&cs=tinysrgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw3fHxzY2hvb2x8ZW58MHx8fHwxNjc1NjY3Nzkz&ixlib=rb-4.0.3&q=80
coverY: 0
---

# 📖 Javascript Practice

## Simple

{% tabs %}
{% tab title="Exercices" %}
Voici 20 exercices de JavaScript :

1. Afficher le nombre de caractères d'une chaîne de caractères.
2. Convertir une chaîne de caractères en majuscules.
3. Convertir une chaîne de caractères en minuscules.
4. Compter le nombre de mots dans une chaîne de caractères.
5. Afficher la position d'un caractère dans une chaîne de caractères.
6. Récupérer une partie d'une chaîne de caractères.
7. Remplacer un caractère dans une chaîne de caractères.
8. Afficher l'heure actuelle.
9. Afficher la date actuelle.
10. Calculer le nombre de jours entre deux dates.
11. Afficher le nombre de secondes restantes jusqu'à la fin de la journée.
12. Afficher le nombre de secondes écoulées depuis le début de la journée.
13. Ajouter des éléments à un tableau.
14. Supprimer des éléments d'un tableau.
15. Trier un tableau
16. Inverser l'ordre d'un tableau.
17. Trouver la somme des éléments d'un tableau.
18. Trouver le nombre maximum d'un tableau.
19. Trouver le nombre minimum d'un tableau.
20. Vérifier si un élément existe dans un tableau.
{% endtab %}

{% tab title="Solutions" %}
Voici les 20 solutions :

1. Afficher le nombre de caractères d'une chaîne de caractères.

```javascript
const string = "Hello World!";
console.log(string.length);
```

2. Convertir une chaîne de caractères en majuscules.

```javascript
const string = "Hello World!";
console.log(string.toUpperCase());
```

3. Convertir une chaîne de caractères en minuscules.

```javascript
const string = "Hello World!";
console.log(string.toLowerCase());
```

4. Compter le nombre de mots dans une chaîne de caractères.

```javascript
const string = "Hello World!";
console.log(string.split(" ").length);
```

5. Afficher la position d'un caractère dans une chaîne de caractères.

```javascript
const string = "Hello World!";
console.log(string.indexOf("o"));
```

6. Récupérer une partie d'une chaîne de caractères.

```javascript
const string = "Hello World!";
console.log(string.slice(0, 5));
```

7. Remplacer un caractère dans une chaîne de caractères.

```javascript
const string = "Hello World!";
console.log(string.replace("!", "?"));
```

8. Afficher l'heure actuelle.

```javascript
console.log(new Date().toLocaleTimeString());
```

9. Afficher la date actuelle.

```javascript
console.log(new Date().toLocaleDateString());
```

10. Calculer le nombre de jours entre deux dates.

```javascript
const date1 = new Date("2022-01-01");
const date2 = new Date("2022-01-31");
console.log((date2 - date1) / (1000 * 60 * 60 * 24) + 1);
```

11. Afficher le nombre de secondes restantes jusqu'à la fin de la journée.

```javascript
const now = new Date();
const endOfDay = new Date(now.getFullYear(), now.getMonth(), now.getDate(), 23, 59, 59, 999);
console.log((endOfDay - now) / 1000);
```

12. Afficher le nombre de secondes écoulées depuis le début de la journée.

```javascript
const now = new Date();
const startOfDay = new Date(now.getFullYear(), now.getMonth(), now.getDate());
console.log((now - startOfDay) / 1000);
```

13. Ajouter des éléments à un tableau.

```c
const array = [1, 2, 3];
array.push(4, 5);
console.log(array);
```

14. Supprimer des éléments d'un tableau.

```c
const array = [1, 2, 3, 4,5]; array.pop(); console.log(array);
```

15. Trier un tableau.

<pre class="language-javascript"><code class="lang-javascript"><strong>const array = [3, 1, 5, 2, 4]; console.log(array.sort());
</strong></code></pre>

16. Inverser l'ordre d'un tableau.

```rust
const array = [1, 2, 3, 4, 5]; console.log(array.reverse());
```

17. Trouver la somme des éléments d'un tableau.

<pre class="language-javascript"><code class="lang-javascript"><strong>const array = [1, 2, 3, 4, 5]; console.log(array.reduce((sum, value) => sum + value, 0));
</strong></code></pre>

18. Trouver le nombre maximum d'un tableau.

```javascript
const array = [1, 2, 3, 4, 5]; console.log(Math.max(...array));
```

19. Trouver le nombre minimum d'un tableau.

<pre class="language-javascript"><code class="lang-javascript"><strong>const array = [1, 2, 3, 4, 5]; console.log(Math.min(...array));
</strong></code></pre>

20. Vérifier si un élément existe dans un tableau.

```javascript
const array = [1, 2, 3, 4, 5]; console.log(array.includes(3));
```
{% endtab %}
{% endtabs %}

## Medium

{% tabs %}
{% tab title="Exercices" %}
Voici 20 exercices de niveau moyen en JavaScript:

1. Créer un objet qui représente une personne avec des propriétés telles que le nom, l'âge, l'adresse, etc.
2. Afficher une propriété d'un objet.
3. Modifier une propriété d'un objet.
4. Ajouter une propriété à un objet.
5. Supprimer une propriété d'un objet.
6. Vérifier si une propriété existe dans un objet.
7. Boucler à travers les propriétés d'un objet.
8. Convertir un nombre en chaîne de caractères.
9. Convertir une chaîne de caractères en nombre.
10. Arrondir un nombre à un nombre spécifique de décimales.
11. Déterminer le type d'un objet.
12. Déterminer si un objet est un tableau.
13. Déterminer si un objet est une fonction.
14. Créer une fonction qui prend des arguments.
15. Créer une fonction qui retourne une valeur.
16. Utiliser des paramètres par défaut dans une fonction.
17. Utiliser des destructurations dans une fonction.
18. Boucler à travers un tableau avec forEach.
19. Boucler à travers un tableau avec map.
20. Filtrer un tableau avec filter.
{% endtab %}

{% tab title="Solutions" %}
1. Créer un objet qui représente une personne avec des propriétés telles que le nom, l'âge, l'adresse, etc.

```javascript
const person = {
  name: "John Doe",
  age: 30,
  address: {
    street: "123 Main St",
    city: "San Francisco",
    state: "CA"
  }
};
console.log(person);
```

2. Afficher une propriété d'un objet.

```javascript
const person = {
  name: "John Doe",
  age: 30
};
console.log(person.name);
```

3. Modifier une propriété d'un objet.

```javascript
const person = {
  name: "John Doe",
  age: 30
};
person.age = 31;
console.log(person.age);
```

4. Ajouter une propriété à un objet.

```javascript
const person = {
  name: "John Doe",
  age: 30
};
person.address = "123 Main St";
console.log(person.address);
```

5. Supprimer une propriété d'un objet.

```javascript
const person = {
  name: "John Doe",
  age: 30,
  address: "123 Main St"
};
delete person.address;
console.log(person);
```

6. Vérifier si une propriété existe dans un objet.

```javascript
const person = {
  name: "John Doe",
  age: 30
};
console.log("address" in person);
```

7. Boucler à travers les propriétés d'un objet.

```javascript
const person = {
  name: "John Doe",
  age: 30,
  address: "123 Main St"
};
for (const property in person) {
  console.log(`${property}: ${person[property]}`);
}
```

8. Convertir un nombre en chaîne de caractères.

```typescript
const number = 123;
console.log(number.toString());
```

9. Convertir une chaîne de caractères en nombre.

```javascript
const string = "123";
console.log(Number(string));
```

10. Arrondir un nombre à un nombre spécifique de décimales.

```javascript
const number = 123.456;
console.log(number.toFixed(2));
```

11. Déterminer le type d'un objet.

```javascript
const array = [1, 2, 3];
console.log(typeof array);
```

12. Déterminer si un objet est un tableau.

```javascript
const array = [1, 2, 3];
console.log(Array.isArray(array));
```

13. Déterminer si un objet est une fonction.

```javascript
const fn = function() {};
console.log(typeof fn === "function");
```

14. Créer une fonction qui prend des arguments.

```javascript
const add = (a, b) => a + b;
console.log(add(1, 2));
```

15. Créer une fonction qui retourne une valeur.

```javascript
const add = (a, b) => a + b;
const result = add(1, 2);
console.log(result);
```

16. Utiliser des paramètres par défaut dans une fonction.

```javascript
const add = (a, b = 0) => a + b;
console.log(add(1));
```

17. Utiliser des destructurations dans une fonction.

```javascript
const add = ({ a, b = 0 }) => a + b;
console.log(add({ a: 1 }));
```

18. Boucler à travers un tableau avec forEach.

```javascript
const array = [1, 2, 3];
array.forEach(value => console.log(value));
```

19. Boucler à travers un tableau avec map.

```javascript
const array = [1, 2, 3];
const mappedArray = array.map(value => value * 2);
console.log(mappedArray);
```

20. Filtrer un tableau avec filter.

```javascript
const array = [1, 2, 3, 4, 5];
const filteredArray = array.filter(value => value % 2 === 0);
console.log(filteredArray);
```
{% endtab %}
{% endtabs %}

