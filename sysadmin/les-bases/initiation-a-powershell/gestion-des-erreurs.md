# Gestion des erreurs

La gestion des erreurs permet de traiter les erreurs qui peuvent survenir lors de l'exécution des commandes dans PowerShell. Il existe plusieurs méthodes pour gérer les erreurs, notamment en utilisant les structures de contrôle telles que `try-catch`, les erreurs d'arrêt (stop errors) et les erreurs sémantiques (terminating errors).

1. `try-catch` : La structure `try-catch` permet de tenter d'exécuter un ensemble de commandes dans un bloc `try`, et de capturer toutes les erreurs qui peuvent survenir dans un bloc `catch`.

Exemple :

```powershell
try {
  Get-ChildItem c:\nonexistentfolder
} catch {
  Write-Output "Error: $_"
}
```

2. Erreurs d'arrêt (stop errors) : Les erreurs d'arrêt sont des erreurs qui interrompent l'exécution d'un script ou d'une commande, avec un message d'erreur standard. Vous pouvez gérer ces erreurs en utilisant la structure `try-catch`.
3. Erreurs sémantiques (terminating errors) : Les erreurs sémantiques sont des erreurs plus graves qui peuvent interrompre l'exécution d'un script ou d'une commande, sans aucune possibilité de récupération. Vous pouvez gérer ces erreurs en utilisant la structure `try-catch`.

En résumé, la gestion des erreurs permet de traiter les erreurs qui peuvent survenir lors de l'exécution des commandes dans PowerShell, en utilisant des structures telles que `try-catch`, les erreurs d'arrêt et les erreurs sémantiques.
