# Structure des commandes

La structure générale d'une commande PowerShell est la suivante:

```
<cmdlet> [-parameterName] <value> [-parameterName <value>] ...
```

Les cmdlets sont les briques de base pour exécuter des tâches dans PowerShell. Ils sont similaires aux commandes dans d'autres shells de commande. Les paramètres permettent de spécifier les options pour le cmdlet en question.

Voici un exemple de commande pour afficher les fichiers dans un répertoire:

```sql
Get-ChildItem -Path C:\MyDirectory
```

Dans cet exemple, `Get-ChildItem` est le cmdlet et `-Path` est un paramètre qui spécifie le chemin du répertoire à afficher. La valeur du paramètre est `C:\MyDirectory`. La commande affichera tous les fichiers dans ce répertoire.
