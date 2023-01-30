# Python Modules et bibliothèques

Les modules et les bibliothèques en Python sont des ensembles de fonctions, classes et variables qui peuvent être utilisés pour ajouter des fonctionnalités à vos programmes. Ils permettent de structurer et de réutiliser facilement le code, et d'éviter la duplication de code.

Les modules sont des fichiers Python contenant des définitions de fonctions, de classes et de variables. Vous pouvez les utiliser en les importants dans votre programme à l'aide de la commande `import`. Par exemple :

```python
import math
print(math.pi)
```

Les bibliothèques sont des ensembles de modules regroupés ensemble. Les bibliothèques les plus courantes en Python sont regroupées dans le système de distribution Python (Python Standard Library). Vous pouvez également installer des bibliothèques tierces pour ajouter des fonctionnalités spécifiques à vos programmes.

Il existe deux types de modules: les modules built-in (intégrés) et les modules externes. Les modules built-in sont inclus avec Python lorsque vous l'installez, ils sont donc disponibles pour tous les programmes Python. Les modules externes, quant à eux, doivent être installés séparément.

Pour utiliser un module externe, vous devez d'abord l'installer en utilisant un gestionnaire de paquet comme pip, par exemple :

```shell
pip install nom_module
```

Ensuite, vous pouvez l'utiliser dans votre programme en l'important :

```python
import nom_module
```

Il est également possible d'importer uniquement une partie d'un module en utilisant la syntaxe `from module import objet`. Par exemple :

```python
from math import pi
print(pi)
```

Voici quelques exemples de modules et de bibliothèques populaires en Python :

1. Le module `math` fournit des fonctions mathématiques courantes telles que `sin`, `cos`, `sqrt`, etc.

```python
import math
print(math.sin(math.pi/2)) # 1.0
```

2. Le module `random` fournit des fonctions pour générer des nombres aléatoires.

```python
import random
print(random.randint(1, 10)) # un entier aléatoire entre 1 et 10
```

3. La bibliothèque `numpy` est une bibliothèque populaire pour le calcul scientifique et numérique en Python. Elle fournit des fonctions pour travailler avec des tableaux multidimensionnels et des opérations mathématiques sur ces tableaux.

```python
import numpy as np
a = np.array([1, 2, 3])
print(a + 2) # [3 4 5]
```
