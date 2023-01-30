# Python Algorithmie

L'algorithmie est l'ensemble des techniques permettant de résoudre un problème de manière efficace et optimale. Il existe différents types d'algorithmes, tels que les algorithmes de tri, de recherche, de parcours de graphe, etc.

Lorsque vous écrivez du code en Python, il est important de comprendre comment fonctionnent les différents algorithmes et de savoir les utiliser efficacement. Cela vous permettra de résoudre des problèmes de manière efficace et de réduire les temps d'exécution de vos programmes.

Voici quelques exemples d'algorithmes couramment utilisés en Python:

1. Tri : L'algorithme de tri le plus courant en Python est le tri à bulle. Il consiste à parcourir la liste à trier plusieurs fois en comparant chaque élément à son voisin, et en échangeant les éléments si nécessaire. Le tri à bulle est un algorithme peu efficace pour les grandes listes, mais il est facile à comprendre et à implémenter.

```python
def tri_bulle(liste):
    n = len(liste)
    for i in range(n):
        for j in range(0, n-i-1):
            if liste[j] > liste[j+1] :
                liste[j], liste[j+1] = liste[j+1], liste[j]
    return liste
```

2. Recherche : L'algorithme de recherche le plus courant en Python est la recherche séquentielle. Il consiste à parcourir la liste élément par élément en comparant chaque élément à celui que l'on cherche. Si l'élément est trouvé, la recherche s'arrête et la fonction renvoie l'index de l'élément. Sinon, la fonction renvoie -1.

```python
def recherche_sequentielle(liste, x):
    for i in range(len(liste)):
        if liste[i] == x:
            return i
    return -1
```

3. Parcours de graphe : L'algorithme de parcours de graphe le plus courant en Python est l'algorithme en largeur d'abord (BFS). Il consiste à parcourir tous les noeuds d'un graphe à partir d'un noeud de départ en utilisant une queue.

```python
from collections import deque

def parcours_en_largeur(graph, start):
    visited = set()
    queue = deque([start])
    while queue:
        vertex = queue.popleft()
        if vertex not in visited:
            visited.add(vertex)
            queue.extend(graph[vertex] - visited)
    return visited
```

L'algorithmie est un domaine de la programmation qui consiste à résoudre des problèmes en utilisant des méthodes logiques et systématiques. Cela implique de comprendre le problème à résoudre, de décomposer ce problème en sous-problèmes plus simples, de développer un plan pour résoudre chaque sous-problème et de mettre en œuvre ce plan en utilisant des structures de données et des algorithmes appropriés.

Il existe de nombreux types d'algorithmes, chacun ayant des caractéristiques et des utilisations différentes. Les algorithmes de tri, par exemple, permettent de classer les données dans un ordre particulier, tandis que les algorithmes de recherche permettent de trouver un élément spécifique dans un ensemble de données. Les algorithmes de parcours permettent de parcourir les données dans un ordre spécifique, tandis que les algorithmes de graphe permettent de trouver des chemins ou des itinéraires dans les graphes.

Il est important de comprendre les performances des différents algorithmes et de choisir celui qui convient le mieux à un cas d'utilisation donné. Pour cela, il est nécessaire de connaître les complexités algorithmiques, notamment la complexité temporelle et la complexité spatiale. La complexité temporelle mesure le temps nécessaire pour exécuter un algorithme en fonction de la taille des données en entrée, tandis que la complexité spatiale mesure l'espace mémoire nécessaire pour stocker les données et les résultats intermédiaires.

Voici quelques exemples d'algorithmes courants en python :

* Tri par sélection :

```python
def selection_sort(arr):
    for i in range(len(arr)):
        min_idx = i
        for j in range(i+1, len(arr)):
            if arr[min_idx] > arr[j]:
                min_idx = j
        arr[i], arr[min_idx] = arr[min_idx], arr[i]
    return arr
```

* Recherche dichotomique :

```python
def binary_search(arr, x):
    low = 0
    high = len(arr) - 1
    mid = 0
 
    while low <= high:
 
        mid = (high + low) // 2
 
        # Check if x is greater, less or equal than mid
        if arr[mid] < x:
            low = mid + 1
 
        # If x is greater, ignore left half
        elif arr[mid] > x:
            high = mid - 1
 
        # If x is smaller, ignore right half
        else:
            return mid
    return -1
```

