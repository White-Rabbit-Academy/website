---
cover: >-
  https://images.unsplash.com/photo-1604134967494-8a9ed3adea0d?crop=entropy&cs=tinysrgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw3fHxzY2hvb2x8ZW58MHx8fHwxNjc1NjY3Nzkz&ixlib=rb-4.0.3&q=80
coverY: 0
---

# 📖 Javascript Practice

## Simple

{% tabs %}
{% tab title="Exercices" %}
Voici 20 exercices de JavaScript avec leurs solutions :

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
20. Trouver le nombre minimum d'un tableau.
{% endtab %}

{% tab title="Solutions" %}
Voici 20 exercices de JavaScript avec leurs solutions :

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



