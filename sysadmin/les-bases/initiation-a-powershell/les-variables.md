# Les variables

Les variables sont des espaces de stockage temporaires pour les données utilisées dans PowerShell. Elles peuvent stocker des valeurs de n'importe quel type, tels que des nombres, des chaînes, des objets, des tableaux, etc.

Pour déclarer une variable, il suffit de spécifier son nom et de lui attribuer une valeur en utilisant le signe `=` :

```powershell
$variableName = "value"
```

Il est également possible de déclarer des variables en utilisant le type de données souhaité :

```powershell
[int]$number = 42
[string]$text = "Hello World"
```

Les variables peuvent être utilisées dans les commandes en y faisant référence par leur nom précédé d'un `$`. Par exemple :

```powershell
$variableName = "value"
Write-Output $variableName
```

En résumé, les variables sont des espaces de stockage temporaires pour les données utilisées dans PowerShell, qui peuvent stocker des valeurs de n'importe quel type. Elles peuvent être déclarées en utilisant leur nom et en leur attribuant une valeur, et peuvent être utilisées dans les commandes en y faisant référence par leur nom.
