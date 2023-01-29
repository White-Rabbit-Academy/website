# Les variables

Les variables en bash sont des conteneurs pour stocker des valeurs, telles que des nombres, des chaînes de caractères ou des tableaux.

Pour déclarer une variable en bash, vous pouvez utiliser le format suivant :

```bash
nom_de_variable=valeur
```

Exemple :

```bash
nom="Alice Snow"
age=20
```

Vous pouvez utiliser la variable en la précédant avec un dollar "$", comme ceci :

```bash
echo "Bonjour, mon nom est $nom et j'ai $age ans."
```

Le résultat de ce code serait :

```bash
Bonjour, mon nom est Alice Snow et j'ai 20 ans.
```

Il existe également des variables d'environnement prédéfinies en bash, telles que `PATH`, `HOME` et `SHELL`, qui contiennent des informations sur le système. Vous pouvez accéder à ces variables en utilisant le même format que pour les variables déclarées, c'est-à-dire en les précédant d'un "$".

Exemple :

```bash
echo "Mon shell actuel est $SHELL."
```

Le résultat de ce code pourrait être :

```
Mon shell actuel est /bin/bash.
```
