# Gestion des modules

La gestion des modules est un aspect important de PowerShell qui permet d'ajouter des fonctionnalités supplémentaires à l'interpréteur. Les modules sont des collections de cmdlets, fonctions, variables et alias qui peuvent être importées et utilisées dans un script PowerShell. Les modules sont généralement stockés dans des fichiers .psm1 ou .dll.

1. Installation de modules : Vous pouvez installer des modules en utilisant la cmdlet `Install-Module`, qui télécharge et installe les modules depuis un dépôt en ligne, tels que PowerShell Gallery ou un emplacement de dépôt personnalisé.

Exemple :

```powershell
Install-Module -Name AzureAD
```

2. Importation de modules : Vous pouvez importer un module en utilisant la cmdlet `Import-Module`, qui permet de charger les cmdlets, fonctions, variables et alias dans la session PowerShell actuelle.

Exemple :

```powershell
Import-Module -Name AzureAD
```

3. Exportation de modules : Vous pouvez exporter un module en créant un fichier .psm1 contenant les cmdlets, fonctions, variables et alias que vous souhaitez partager. Ce fichier peut être publié sur un dépôt en ligne pour être téléchargé et installé par d'autres utilisateurs.

En résumé, la gestion des modules permet d'ajouter des fonctionnalités supplémentaires à l'interpréteur PowerShell en installant, important et exportant des modules.
