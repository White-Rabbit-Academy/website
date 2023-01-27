# Les expressions régulières

### Les expressions régulières

Les expressions régulières (ou regex) sont un moyen de décrire une séquence de caractères à rechercher dans un texte. Elles permettent de vérifier si une chaîne de caractères correspond à un certain format ou contient une certaine sous-chaîne. Les expressions régulières sont utilisées dans de nombreux langages de programmation, ainsi que dans de nombreux outils de traitement de texte et de recherche.

Les grand principes des expressions régulières incluent :

* La capacité à utiliser des caractères génériques tels que "." pour correspondre à n'importe quel caractère unique, et "\*" pour correspondre à zéro ou plusieurs occurrences d'un caractère.
* La capacité à utiliser des séquences de caractères encadrée par "\[]" pour correspondre à n'importe quel caractère à l'intérieur de ces crochets.
* La capacité à utiliser des séquences de caractères encadrée par "()" pour créer des groupes de capture pour faciliter l'extraction de sous-chaînes correspondant à la regex.
* La capacité à utiliser des modificateurs tels que "^" et "$" pour définir le début et la fin de la chaîne de caractères correspondante.

### Exemples :&#x20;

Voici quelques exemples d'expressions régulières avec une explication détaillée :

1. Vérifier si une chaîne de caractères contient un numéro de téléphone américain valide :

```regex
^(1\s|1|)?((\(\d{3}\))|\d{3})(\-|\s)?(\d{3})(\-|\s)?(\d{4})$
```

* `^` indique le début de la chaîne de caractères.
* `(1\s|1|)?` permet de correspondre à un éventuel indicatif de pays "1" ou "1 " au début de la chaîne.
* `((\(\d{3}\))|\d{3})` permet de correspondre à un groupe de 3 chiffres entouré de parenthèses ou simplement 3 chiffres.
* `(\-|\s)?` permet de correspondre à un éventuel tiret ou espace après le groupe de 3 chiffres.
* `(\d{3})` permet de correspondre à un groupe de 3 chiffres.
* `(\-|\s)?` permet de correspondre à un éventuel tiret ou espace après le groupe de 3 chiffres.
* `(\d{4})` permet de correspondre à un groupe de 4 chiffres.
* `$` indique la fin de la chaîne de caractères.

2. Extraire tous les mots commençant par une majuscule dans une phrase:

```regex
\b[A-Z][a-z]*\b
```

* `\b` indique un début ou une fin de mot.
* `[A-Z]` permet de correspondre à une majuscule.
* `[a-z]*` permet de correspondre à zéro ou plusieurs minuscules.
* `\b` indique un début ou une fin de mot.

3. Vérifier si une adresse e-mail est valide :

```regex
^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$
```

* `^` indique le début de la chaîne de caractères.
* `[a-zA-Z0-9._%+-]+` permet de correspondre à une série de caractères alphanumériques, des points, des tirets, des pourcentages, des plus et des moins.
* `@` permet de correspondre à un symbole "@".
* `[a-zA-Z0-9.-]+` permet de correspondre à une série de caractères alphanumériques, des points et des tirets.
* `\.` permet de correspondre à un point.
* `[a-zA-Z]{2,}` permet de correspondre à au moins 2 caractères alphabétiques.
* `$` indique la fin de la chaîne de caractères.

4. Remplacer tous les espaces multiples dans une chaîne de caractères par un seul espace :

```regex
\s+
```

* `\s` permet de correspondre à un espace.
* `+` permet de correspondre à un ou plusieurs espaces.

5. Extraire tous les numéros d'une chaîne de caractères :

```regex
\d+
```

* `\d` permet de correspondre à un chiffre.
* `+` permet de correspondre à un ou plusieurs chiffres.

Il est important de noter que ces exemples sont très simplifiés et peuvent ne pas être suffisamment robustes pour un usage réel. Il est également important de vérifier si les expressions régulières utilisées sont compatibles avec le langage de programmation ou le logiciel utilisé.

{% hint style="info" %}
Vas sur [https://www.regextester.com/](https://www.regextester.com/) pour tester tes regex :thumbsup:
{% endhint %}
