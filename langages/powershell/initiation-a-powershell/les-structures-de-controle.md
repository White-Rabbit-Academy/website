# Les structures de contrôle

Les structures de contrôle permettent de contrôler l'exécution des commandes dans PowerShell. Il en existe plusieurs types, tels que les conditions, les boucles et les sauts.

1. Les conditions : Les conditions permettent de tester une expression pour déterminer si elle est vraie ou fausse, et d'exécuter des commandes en conséquence. Les structures de condition courantes sont `if`, `if-else` et `switch`.

Exemple :

```powershell
$number = 42
if ($number -gt 10) {
  Write-Output "Number is greater than 10"
}
```

2. Les boucles : Les boucles permettent de répéter un ensemble de commandes plusieurs fois, en utilisant des structures telles que `for`, `foreach`, `while` et `do-while`.

Exemple :

```powershell
for ($i=0; $i -lt 5; $i++) {
  Write-Output $i
}
```

3. Les sauts : Les sauts permettent d'interrompre une boucle ou une structure de contrôle en cours d'exécution, en utilisant des instructions telles que `break` et `continue`.

En résumé, les structures de contrôle permettent de contrôler l'exécution des commandes dans PowerShell, en utilisant des conditions pour tester des expressions, des boucles pour répéter un ensemble de commandes plusieurs fois, et des sauts pour interrompre une boucle ou une structure de contrôle en cours d'exécution.
