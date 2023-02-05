# DML – La gestion des données

DML signifie Data Manipulation Language et c'est une partie du langage SQL qui permet de manipuler les données dans les bases de données relationnelles, telles que les tables. Il sert à lire, insérer, mettre à jour et supprimer des données dans les tables.

Les principales commandes DML sont :

1. SELECT : utilisée pour récupérer des données à partir d'une table. Exemple :

```sql
SELECT name, salary FROM employees;
```

2. INSERT INTO : utilisée pour insérer de nouvelles lignes de données dans une table. Exemple :

```sql
INSERT INTO employees (id, name, salary, hire_date)
VALUES (1, 'John Doe', 50000, '2022-01-01');
```

3. UPDATE : utilisée pour mettre à jour les données existantes dans une table. Exemple :

```sql
UPDATE employees
SET salary = 55000
WHERE id = 1;
```

4. DELETE : utilisée pour supprimer des lignes de données d'une table. Exemple :

```sql
DELETE FROM employees
WHERE id = 1;
```

Ces commandes sont utilisées pour manipuler les données dans les bases de données et sont essentielles pour le développement d'applications qui interagissent avec les bases de données.

### Exercices

{% tabs %}
{% tab title="Select" %}
1. Exemple simple : Sélection de toutes les colonnes pour toutes les lignes de la table "Personnes".
2. Exemple intermédiaire : Sélection de la colonne "Nom" et "Prénom" pour toutes les lignes de la table "Personnes" où la colonne "ID" est égale à 1.
3. Exemple avancé : Sélection de la colonne "Nom" et "Prénom" pour toutes les lignes de la table "Personnes" où la colonne "Nom" commence par "D" et ordonnées par la colonne "Nom".
{% endtab %}

{% tab title="Solutions" %}
1. Exemple simple : Sélection de toutes les colonnes pour toutes les lignes de la table "Personnes".

```sql
SELECT * FROM Personnes;
```

2. Exemple intermédiaire : Sélection de la colonne "Nom" et "Prénom" pour toutes les lignes de la table "Personnes" où la colonne "ID" est égale à 1.

```sql
SELECT Nom, Prenom FROM Personnes
WHERE ID = 1;
```

3. Exemple avancé : Sélection de la colonne "Nom" et "Prénom" pour toutes les lignes de la table "Personnes" où la colonne "Nom" commence par "D" et ordonnées par la colonne "Nom".

```sql
SELECT Nom, Prenom FROM Personnes
WHERE Nom LIKE 'D%'
ORDER BY Nom;
```
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Insert" %}
1. Exemple simple : Insertion d'une nouvelle ligne dans la table "Personnes".
2. Exemple intermédiaire : Insertion de plusieurs nouvelles lignes dans la table "Personnes".
3. Exemple avancé : Insertion d'une nouvelle ligne dans la table "Orders" en utilisant une sous-requête pour obtenir la valeur pour la colonne "Client\_ID".
{% endtab %}

{% tab title="Solutions" %}
1. Exemple simple : Insertion d'une nouvelle ligne dans la table "Personnes".

```sql
INSERT INTO Personnes (ID, Nom, Prenom)
VALUES (1, 'Dupont', 'Jean');
```

2. Exemple intermédiaire : Insertion de plusieurs nouvelles lignes dans la table "Personnes".

```sql
INSERT INTO Personnes (ID, Nom, Prenom)
VALUES (2, 'Durand', 'Marie'),
       (3, 'Martin', 'Luc');
```

3. Exemple avancé : Insertion d'une nouvelle ligne dans la table "Orders" en utilisant une sous-requête pour obtenir la valeur pour la colonne "Client\_ID".

```sql
INSERT INTO Orders (ID, Date, Client_ID, Montant)
VALUES (1, '2022-01-01', 
        (SELECT ID FROM Client WHERE Nom = 'Dupont'),
        100.0);
```
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Update" %}
1. Exemple simple : Mise à jour de la colonne "Prenom" pour toutes les lignes de la table "Personnes" où la colonne "ID" est égale à 1.
2. Exemple intermédiaire : Mise à jour de la colonne "Montant" pour toutes les lignes de la table "Orders" en ajoutant 10 à la valeur actuelle.
3. Exemple avancé : Mise à jour de la colonne "Prenom" pour toutes les lignes de la table "Personnes" en utilisant une sous-requête pour obtenir la nouvelle valeur.
{% endtab %}

{% tab title="Solutions" %}
1. Exemple simple : Mise à jour de la colonne "Prenom" pour toutes les lignes de la table "Personnes" où la colonne "ID" est égale à 1.

```sql
UPDATE Personnes
SET Prenom = 'Jacques'
WHERE ID = 1;
```

2. Exemple intermédiaire : Mise à jour de la colonne "Montant" pour toutes les lignes de la table "Orders" en ajoutant 10 à la valeur actuelle.

```sql
UPDATE Orders
SET Montant = Montant + 10;
```

3. Exemple avancé : Mise à jour de la colonne "Prenom" pour toutes les lignes de la table "Personnes" en utilisant une sous-requête pour obtenir la nouvelle valeur.

```sql
UPDATE Personnes
SET Prenom = (SELECT Prenom FROM Personnes WHERE ID = 2)
WHERE ID = 1;
```
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Delete" %}
1. Exemple simple : Suppression de la ligne de la table "Personnes" où la colonne "ID" est égale à 1.
2. Exemple intermédiaire : Suppression de toutes les lignes de la table "Orders" où la colonne "Montant" est inférieure à 50.
3. Exemple avancé : Suppression de toutes les lignes de la table "Orders" en utilisant une sous-requête pour déterminer les lignes à supprimer.
{% endtab %}

{% tab title="Solutions" %}
1. Exemple simple : Suppression de la ligne de la table "Personnes" où la colonne "ID" est égale à 1.

```sql
DELETE FROM Personnes
WHERE ID = 1;
```

2. Exemple intermédiaire : Suppression de toutes les lignes de la table "Orders" où la colonne "Montant" est inférieure à 50.

```sql
DELETE FROM Orders
WHERE Montant < 50;
```

3. Exemple avancé : Suppression de toutes les lignes de la table "Orders" en utilisant une sous-requête pour déterminer les lignes à supprimer.

```sql
DELETE FROM Orders
WHERE Client_ID IN (SELECT ID FROM Client WHERE Ville = 'Paris');
```
{% endtab %}
{% endtabs %}
