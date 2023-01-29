# Administration à distance

L'administration à distance permet d'exécuter des commandes PowerShell sur un ordinateur distant, en utilisant les protocoles de réseau tels que WS-Management ou SMB. Il existe plusieurs méthodes pour administrer à distance avec PowerShell, telles que :

1. `Invoke-Command` : La cmdlet `Invoke-Command` permet d'exécuter des commandes sur un ou plusieurs ordinateurs distants. Vous pouvez spécifier les ordinateurs distants en utilisant un nom d'hôte ou une adresse IP, ou en utilisant un fichier CSV ou une liste d'ordinateurs.

Exemple :

```powershell
Invoke-Command -ComputerName server01 -ScriptBlock {Get-Process}
```

2. `Enter-PSSession` : La cmdlet `Enter-PSSession` permet de créer une session interactieve avec un ordinateur distant, pour exécuter des commandes en mode interactif sur ce dernier.

Exemple :

```powershell
Enter-PSSession -ComputerName server01
```

3. `New-PSSession` : La cmdlet `New-PSSession` permet de créer une session distante avec un ordinateur distant, pour exécuter des commandes à distance de manière asynchrone.

Exemple :

```powershell
$session = New-PSSession -ComputerName server01
Invoke-Command -Session $session -ScriptBlock {Get-Process}
```

En résumé, l'administration à distance permet d'exécuter des commandes PowerShell sur un ordinateur distant, en utilisant des cmdlets telles que `Invoke-Command`, `Enter-PSSession` et `New-PSSession`.
