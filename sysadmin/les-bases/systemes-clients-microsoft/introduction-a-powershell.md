---
cover: >-
  https://images.unsplash.com/photo-1635606511031-6ef8c6cbf9f9?crop=entropy&cs=tinysrgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw4fHx0ZXJtaW5hbCUyMHBjfGVufDB8fHx8MTY3NDgzNzg1MA&ixlib=rb-4.0.3&q=80
coverY: 0
---

# Introduction à PowerShell

<figure><img src="../../../.gitbook/assets/say-what-meme.jpg" alt=""><figcaption></figcaption></figure>

PowerShell est un interpréteur de ligne de commande développé par Microsoft pour les systèmes d'exploitation Windows. Il permet aux utilisateurs de lancer des commandes et de créer des scripts pour automatiser des tâches courantes telles que la gestion des utilisateurs, des ordinateurs et des services réseau.

Voici quelques exemples de commandes de base de PowerShell :

* Pour afficher le nom d'utilisateur actuel : `echo $env:username`
* Pour afficher la liste des processus en cours d'exécution : `Get-Process`
* Pour arrêter un processus spécifique : `Stop-Process -Name "nom_du_processus"`
* Pour afficher la liste des services en cours d'exécution : `Get-Service`
* Pour démarrer un service spécifique : `Start-Service -Name "nom_du_service"`

Apprendre à utiliser PowerShell est utile, car cela permet aux administrateurs système et aux développeurs d'automatiser des tâches répétitives et d'interagir de manière programmatique avec les systèmes Windows. Cela peut également aider à résoudre des problèmes plus rapidement et plus efficacement.



## Exercices :

1. Afficher les informations de base de votre système : Utilisez les commandes `Get-ComputerInfo` pour afficher les informations de base de votre système telles que le nom d'hôte, la version de Windows, la mémoire et le processeur.
2. Gérer les processus : Utilisez les commandes `Get-Process` pour afficher la liste des processus en cours d'exécution, `Stop-Process` pour arrêter un processus spécifique, et `Start-Process` pour démarrer un processus spécifique.
3. Gérer les services : Utilisez les commandes `Get-Service` pour afficher la liste des services en cours d'exécution, `Stop-Service` pour arrêter un service spécifique, et `Start-Service` pour démarrer un service spécifique.
4. Gérer les utilisateurs : Utilisez les commandes `Get-LocalUser` pour afficher la liste des utilisateurs locaux sur votre système, `New-LocalUser` pour créer un nouvel utilisateur local, et `Remove-LocalUser` pour supprimer un utilisateur local.
5. Créer un script : Utilisez PowerShell pour créer un script qui automatise une tâche courante, comme la sauvegarde de fichiers importants sur un disque réseau ou l'envoi d'un e-mail automatisé.

Notez qu'il est important de faire les exercices dans un environnement de test pour eviter tout impact sur un environnement de production.

{% hint style="info" %}
Powershell en détail, c'est pour plus tard !
{% endhint %}
