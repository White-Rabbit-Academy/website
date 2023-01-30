# Python Erreurs et débogage

Le point 5 concerne les erreurs et le débogage en programmation. Il est important de comprendre comment gérer les erreurs qui peuvent survenir lors de l'exécution de votre code, ainsi que les outils et les techniques utilisés pour les détecter et les corriger.

Il existe deux types d'erreurs courantes en Python : les erreurs de syntaxe et les erreurs d'exécution. Les erreurs de syntaxe se produisent lorsque le code est mal écrit, par exemple en oubliant un point-virgule ou en utilisant des parenthèses incorrectes. Les erreurs d'exécution, quant à elles, se produisent lorsque le code est correctement écrit, mais qu'il rencontre une situation imprévue lors de son exécution, comme une division par zéro ou l'accès à un élément d'une liste qui n'existe pas.

Pour gérer les erreurs en Python, vous pouvez utiliser les instructions try-except. La syntaxe est la suivante :

```python
try:
    # code qui peut générer une erreur
except ExceptionType:
    # code à exécuter en cas d'erreur
```

Il est également possible de spécifier plusieurs types d'erreurs à traiter avec une instruction except multiple :

```python
try:
    # code qui peut générer une erreur
except ExceptionType1:
    # code à exécuter en cas d'erreur de type 1
except ExceptionType2:
    # code à exécuter en cas d'erreur de type 2
```

Enfin, il est possible d'utiliser l'instruction finally qui permet d'exécuter du code quel que soit le résultat de l'instruction try :

```python
try:
    # code qui peut générer une erreur
except ExceptionType:
    # code à exécuter en cas d'erreur
finally:
    # code à exécuter dans tous les cas
```

Pour le débogage, il existe plusieurs outils intégrés à Python, tels que :

* `print()` pour afficher des informations à des endroits précis de votre code
* `assert` pour vérifier une condition et lever une erreur si elle n'est pas remplie
* `pdb`, le débogueur intégré de python

Voici un exemple d'utilisation de try-except pour gérer une erreur de division par zéro :

```python
try:
    result = 5 / 0
except ZeroDivisionError:
    print("Vous ne pouvez pas diviser un nombre par zéro.")
```

Utilisation de l'instruction `assert` pour vérifier des conditions :

```python
x = -1
assert x > 0, "x doit être positif"
```

Utilisation de la fonction `print()` pour afficher des informations de débogage :

```python
def ma_fonction(x):
    print("Entrée :", x)
    resultat = x * 2
    print("Sortie :", resultat)
    return resultat
```

Utilisation de la bibliothèque `pdb` pour le débogage interactif :

```python
import pdb

x = [1, 2, 3]
y = 4

pdb.set_trace()
resultat = y + x
print(resultat)
```

Il est important de noter que ces exemples ne couvrent qu'une partie des fonctionnalités de débogage disponibles en Python, mais ils peuvent vous donner une idée de ce à quoi ils ressemblent et comment ils fonctionnent. Il est également important de noter que le débogage est un processus continu et en évolution au cours du développement d'un projet, il est donc important de s'y consacrer régulièrement pour éviter les bugs dans le code.
