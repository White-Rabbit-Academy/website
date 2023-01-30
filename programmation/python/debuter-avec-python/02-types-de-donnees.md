# Python Types de données

Il est important de comprendre les différentes options disponibles pour stocker et manipuler des données dans vos programmes.

Les structures de données les plus courantes en Python sont les listes, les tuples et les dictionnaires.

Les listes sont similaires aux tableaux en C ou en Java. Elles sont utilisées pour stocker une série d'éléments de même type. Les listes en Python peuvent contenir des éléments de n'importe quel type, y compris d'autres listes. Les éléments d'une liste peuvent être accédés en utilisant leur index, qui est leur position dans la liste. Par exemple, la première valeur d'une liste a un index de 0.

Les tuples sont similaires aux listes, mais ils sont immuables. Une fois qu'un tuple a été créé, il ne peut plus être modifié. Les tuples sont souvent utilisés pour stocker des données qui ne doivent pas être modifiées, comme des coordonnées géographiques.

Les dictionnaires sont similaires aux tableaux associatifs en PHP ou aux objets en JavaScript. Ils sont utilisés pour stocker des données sous forme de clés et de valeurs. Les clés peuvent être de n'importe quel type immutable (comme une chaîne ou un nombre), tandis que les valeurs peuvent être de n'importe quel type. Les valeurs d'un dictionnaire peuvent être accédées en utilisant leur clé.

Il est important de comprendre les avantages et les inconvénients de chaque structure de données et de savoir quand utiliser l'une ou l'autre. Il est également important de savoir comment parcourir, trier et manipuler ces structures de données pour pouvoir les utiliser efficacement dans vos programmes.

Il existe également des structures de données plus avancées en Python, comme les ensembles, les itérables et les générateurs, qui peuvent être utilisées pour des scénarios spécifiques. Il est important de savoir comment utiliser ces structures de données pour pouvoir les utiliser efficacement dans vos programmes.

En résumé, comprendre les différentes structures de données de base en Python, comme les listes, les tuples et les dictionnaires, est important pour stocker et manipuler des données efficacement dans vos programmes. Il est également important de savoir comment parcourir, trier et manipuler ces structures de données pour pouvoir les utiliser efficacement dans vos programmes. Il faut également connaitre les structures de données avancées pour des scénarios spécifiques.

Les ensembles sont similaires aux ensembles mathématiques, ils sont utilisés pour stocker des éléments uniques. Les ensembles sont similaires aux listes ou aux tuples, mais ils n'ont pas d'ordre défini et les éléments ne peuvent pas se répéter. Les ensembles sont souvent utilisés pour vérifier si un élément est déjà présent dans un ensemble ou pour supprimer des doublons d'une liste.

Les itérables sont des objets qui peuvent être utilisés dans une boucle "for" pour parcourir tous les éléments. Les listes, les tuples, les dictionnaires et les ensembles sont tous des itérables, mais il existe d'autres types d'itérables tels que les fichiers et les chaînes de caractères.

Les générateurs sont des objets qui peuvent être utilisés pour créer des itérables de manière efficace. Les générateurs sont souvent utilisés pour créer des itérables qui ne peuvent être stockés en mémoire, comme des séquences infinies ou des séquences très grandes. Les générateurs peuvent être créés en utilisant des fonctions génératrices ou des expressions génératrices.

En résumé, les structures de données avancées, comme les ensembles, les itérables et les générateurs, offrent des fonctionnalités supplémentaires pour des scénarios spécifiques. Les ensembles sont utilisés pour stocker des éléments uniques, les itérables pour parcourir tous les éléments d'un objet et les générateurs pour créer des itérables de manière efficace. Il est important de comprendre ces structures de données avancées et de savoir quand les utiliser pour pouvoir les utiliser efficacement dans vos programmes.

Les ensembles :

```python
# création d'un ensemble
mon_ensemble = set([1, 2, 3])

# ajout d'un élément
mon_ensemble.add(4)

# suppression d'un élément
mon_ensemble.remove(2)

# vérification de la présence d'un élément
print(3 in mon_ensemble) # True

# suppression des doublons d'une liste
ma_liste = [1, 2, 3, 2, 1]
ma_liste = list(set(ma_liste)) # [1, 2, 3]

```

Les itérables :

```python
# boucle for sur une liste
ma_liste = [1, 2, 3]
for element in ma_liste:
    print(element) # 1, 2, 3

# boucle for sur un tuple
mon_tuple = (1, 2, 3)
for element in mon_tuple:
    print(element) # 1, 2, 3

# boucle for sur un dictionnaire
mon_dictionnaire = {'a': 1, 'b': 2, 'c': 3}
for cle, valeur in mon_dictionnaire.items():
    print(cle, valeur) # 'a' 1, 'b' 2, 'c' 3

# boucle for sur un ensemble
mon_ensemble = set([1, 2, 3])
for element in mon_ensemble:
    print(element) # 1, 2, 3

```

Les générateurs :

```python
# générateur avec une fonction génératrice
def mon_generateur():
    i = 0
    while i < 3:
        yield i
        i += 1

# utilisation du générateur
for element in mon_generateur():
    print(element) # 0, 1, 2

# générateur avec une expression génératrice
mon_generateur = (i for i in range(3))

# utilisation du générateur
for element in mon_generateur:
    print(element) # 0, 1, 2

```

Il est important de noter que ces exemples sont des exemples simples pour illustrer le fonctionnement de chacun de ces structures de données. Il existe de nombreuses autres fonctionnalités et utilisations possibles pour chacune d'entre elles. Il est donc important de continuer à explorer et à expérimenter avec ces structures de données pour les comprendre et les utiliser efficacement dans vos programmes.
