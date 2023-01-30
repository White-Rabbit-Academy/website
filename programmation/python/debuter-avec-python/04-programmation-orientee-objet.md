# Python Programmation Orientée Objet

La programmation orientée objet (POO) est un paradigme de programmation qui permet de modéliser des objets du monde réel dans un programme informatique. Les objets sont des instances de classes, qui définissent leur état (attributs) et leur comportement (méthodes). En utilisant la POO, on peut organiser le code de manière plus structurée, réutiliser des morceaux de code, et simuler des interactions entre les objets.

Voici les concepts clés de la POO en Python :

1. Les classes : une classe est un modèle pour créer des objets. Elle définit les attributs et les méthodes de ces objets. On peut définir une classe en utilisant le mot-clé "class", suivi du nom de la classe. Par exemple :

```python
class MaClasse:
    pass
```

2. Les objets : un objet est une instance d'une classe. On peut créer un objet en utilisant le nom de la classe suivi d'une paire de parenthèses. Par exemple :

```python
mon_objet = MaClasse()
```

3. Les attributs : un attribut est une variable qui décrit l'état d'un objet. On peut définir des attributs à l'intérieur d'une classe en utilisant le mot-clé "self" pour accéder à l'objet courant. Par exemple :

```python
class MaClasse:
    def __init__(self):
        self.attribut = "valeur"
```

4. Les méthodes : une méthode est une fonction qui décrit le comportement d'un objet. On peut définir des méthodes à l'intérieur d'une classe en utilisant le mot-clé "def" suivi du nom de la méthode et des paramètres. On utilise également "self" pour accéder à l'objet courant. Par exemple :

```python
class MaClasse:
    def __init__(self):
        self.attribut = "valeur"

    def ma_methode(self):
        print(self.attribut)
```

5. L'héritage : l'héritage permet de définir une classe en utilisant une classe existante comme modèle. La classe héritée peut utiliser tous les attributs et méthodes de la classe parente, et ajouter des attributs et des méthodes supplémentaires. Par exemple :

```python
class MaClasseFille(MaClasse):
    def ma_methode_fille(self):
        print("Je suis une méthode de la classe fille")
```

La programmation orientée objet (POO) est un paradigme de programmation qui permet de structurer le code en utilisant des objets qui ont des propriétés et des méthodes. Cela permet de créer des programmes plus modulaires et réutilisables.

Les classes sont utilisées pour définir les objets dans la POO. Une classe est un modèle pour les objets qui ont les mêmes propriétés et les mêmes méthodes. Les objets créés à partir d'une classe sont appelés instances de la classe.

Parmi les concepts importants de la POO, on peut citer :

* L'encapsulation : cela permet de cacher les détails d'implémentation d'un objet et de ne laisser visible que les propriétés et les méthodes nécessaires à l'utilisation de cet objet.
* L'héritage : cela permet de créer des classes qui héritent des propriétés et des méthodes d'une classe parente. Cela permet de réutiliser du code et de créer des hiérarchies de classes.
* La polymorphisme : cela permet d'utiliser des objets de différentes classes de manière interchangeable, en utilisant une interface commune.

Voici des exemples de code pour illustrer les concepts de la POO :

* Encapsulation :

```python
class CompteBancaire:
    def __init__(self, solde):
        self.__solde = solde

    def get_solde(self):
        return self.__solde

    def set_solde(self, solde):
        self.__solde = solde

compte = CompteBancaire(1000)
print(compte.get_solde()) # Affiche 1000
compte.set_solde(2000)
print(compte.get_solde()) # Affiche 2000

```

* Héritage :

```python
class Personne:
    def __init__(self, nom, prenom):
        self.nom = nom
        self.prenom = prenom

    def afficher(self):
        print(f"{self.prenom} {self.nom}")

class Etudiant(Personne):
    def __init__(self, nom, prenom, matricule):
        Personne.__init__(self, nom, prenom)
        self.matricule = matricule

    def afficher(self):
        Personne.afficher(self)
        print(f"Matricule : {self.matricule}")

etudiant = Etudiant("Dupont", "Jean", "abc123")
etudiant.afficher()

```

La programmation orientée objet (POO) est un paradigme de programmation qui permet de structurer le code en utilisant des objets. Chaque objet est une instance d'une classe qui définit des propriétés (ou attributs) et des méthodes. Les propriétés décrivent les caractéristiques de l'objet, tandis que les méthodes décrivent les actions que l'objet peut effectuer.

Les classes peuvent hériter les propriétés et les méthodes d'autres classes, ce qui permet de créer des hiérarchies d'objets. Les classes filles peuvent surcharger ou étendre les propriétés et les méthodes de leur classe parente.

Pour créer une classe en Python, on utilise le mot-clé `class` suivi du nom de la classe. La définition de la classe est indiquée entre des accolades.

Voici un exemple de classe `Voiture` qui possède des propriétés `marque` et `couleur` ainsi qu'une méthode `demarrer()`.

```python
class Voiture:
    def __init__(self, marque, couleur):
        self.marque = marque
        self.couleur = couleur

    def demarrer(self):
        print(f"La voiture {self.marque} de couleur {self.couleur} démarre.")

ma_voiture = Voiture("Peugeot", "rouge")
ma_voiture.demarrer()
# La sortie sera : La voiture Peugeot de couleur rouge démarre.

```

Le mot-clé `self` est utilisé pour faire référence à l'instance de la classe elle-même. Il est utilisé dans les méthodes pour accéder aux propriétés de l'objet et pour appeler d'autres méthodes de l'objet.

La méthode `__init__` est une méthode spéciale appelée constructeur qui est automatiquement appelée lorsqu'une nouvelle instance de la classe est créée. Elle permet d'initialiser les propriétés de l'objet.

Pour créer une nouvelle instance d'une classe, on utilise le nom de la classe suivi de parenthèses. Les arguments passés à ces parenthèses sont transmis au constructeur de la classe.

Enfin, on peut créer des classes filles qui héritent des propriétés et des méthodes de leur classe parente en utilisant le mot-clé `super()` pour appeler le constructeur de la classe parente.

```python
class VoitureElectrique(Voiture):
    def __init__(self, marque, couleur, batterie):
        super().__init__(marque, couleur)
        self.b
```

