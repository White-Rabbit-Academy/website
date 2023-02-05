# DDL – La gestion des tables

DDL signifie Data Definition Language et c'est une partie du langage SQL qui permet de gérer les structures de données dans les bases de données relationnelles, telles que les tables. Il sert à créer, modifier ou supprimer des tables et d'autres structures de données telles que les vues, les index et les contraintes.

Les principales commandes DDL sont :

1. CREATE TABLE : utilisée pour créer une nouvelle table avec une structure de colonnes et de types de données définis. Exemple :

```sql
CREATE TABLE employees (
  id INT PRIMARY KEY,
  name VARCHAR(50),
  salary DECIMAL(10, 2),
  hire_date DATE
);
```

2. ALTER TABLE : utilisée pour modifier la structure d'une table existante en ajoutant ou supprimant des colonnes, en modifiant le type de données d'une colonne, etc. Exemple :

```sql
ALTER TABLE employees
ADD address VARCHAR(100);
```

3. DROP TABLE : utilisée pour supprimer une table existante avec toutes ses données. Exemple :

```sql
DROP TABLE employees;
```

4. TRUNCATE TABLE : utilisée pour vider les données d'une table sans la supprimer. Exemple :

```sql
TRUNCATE TABLE employees;
```

Ces commandes sont utilisées pour gérer les structures de données dans les bases de données et sont essentielles pour le développement de bases de données robustes et fiables.

### Exercices

{% tabs %}
{% tab title="Create Table" %}
* Exemple simple : Création d'une table "Personnes" avec les colonnes "ID", "Nom" et "Prénom".
* Exemple intermédiaire : Création d'une table "Orders" avec les colonnes "ID", "Date", "Client\_ID" et "Montant", avec une clé étrangère sur la table "Client".
* Exemple avancé : Création d'une table "Employés" avec les colonnes "ID", "Nom", "Prénom", "Adresse" et "Date d'embauche", avec une contrainte sur la colonne "Date d'embauche" pour ne pas permettre les dates antérieures à 2000-01-01.
{% endtab %}

{% tab title="Solutions" %}
```sql
CREATE TABLE Personnes (
  ID int primary key,
  Nom varchar(255),
  Prenom varchar(255)
);
```

2. Exemple intermédiaire : Création d'une table "Orders" avec les colonnes "ID", "Date", "Client\_ID" et "Montant", avec une clé étrangère sur la table "Client".

```sql
CREATE TABLE Orders (
  ID int primary key,
  Date date,
  Client_ID int,
  Montant float,
  foreign key (Client_ID) references Client(ID)
);
```

3. Exemple avancé : Création d'une table "Employés" avec les colonnes "ID", "Nom", "Prénom", "Adresse" et "Date d'embauche", avec une contrainte sur la colonne "Date d'embauche" pour ne pas permettre les dates antérieures à 2000-01-01.

```sql
CREATE TABLE Employes (
  ID int primary key,
  Nom varchar(255),
  Prenom varchar(255),
  Adresse varchar(255),
  Date_Embauche date,
  constraint Date_Embauche_Check check (Date_Embauche >= '2000-01-01')
);
```
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Alter table" %}
1. Exemple simple : Ajout d'une colonne "Adresse" à la table "Personnes".
2. Exemple intermédiaire : Modification de la colonne "Montant" de la table "Orders" pour changer sa taille en float.
3. Exemple avancé : Suppression de la colonne "Adresse" et ajout d'une colonne "Ville" à la table "Employés".
{% endtab %}

{% tab title="Solution" %}
1. Exemple simple : Ajout d'une colonne "Adresse" à la table "Personnes".

```sql
ALTER TABLE Personnes
ADD Adresse varchar(255);
```

2. Exemple intermédiaire : Modification de la colonne "Montant" de la table "Orders" pour changer sa taille en float.

```sql
ALTER TABLE Orders
ALTER COLUMN Montant float;
```

3. Exemple avancé : Suppression de la colonne "Adresse" et ajout d'une colonne "Ville" à la table "Employés".

```sql
ALTER TABLE Employes
DROP COLUMN Adresse,
ADD Ville varchar(255);
```
{% endtab %}
{% endtabs %}
