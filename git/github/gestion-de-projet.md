---
cover: >-
  https://images.unsplash.com/photo-1531403009284-440f080d1e12?crop=entropy&cs=tinysrgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHwxMHx8UHJvamV0JTIwbWFuYWdtZW50fGVufDB8fHx8MTY3NDgzMzE4NA&ixlib=rb-4.0.3&q=80
coverY: 0
---

# 📚 Gestion de projet

## Les bases

GitHub peut être utilisé comme outil de gestion de projet en utilisant des fonctionnalités telles que les "issues" et les "pull requests".

Les "issues" peuvent être utilisées pour signaler des bugs, demander des fonctionnalités ou discuter de questions liées au développement du projet. Les utilisateurs peuvent assigner des tâches à des membres de l'équipe, ajouter des étiquettes pour organiser les tâches et suivre l'avancement du projet.

Les "pull requests" (ou "PR") permettent aux développeurs de soumettre des modifications au code source du projet. Les membres de l'équipe peuvent ensuite discuter et approuver les modifications avant qu'elles ne soient intégrées au code principal. Cela permet aux membres de l'équipe de travailler ensemble pour maintenir la qualité et la stabilité du code.

Exemple de management :

* Vous êtes à la tête d'une équipe de développement de logiciel qui utilise GitHub pour gérer un projet.
* Vous utilisez les "issues" pour créer des tâches pour chaque membre de l'équipe, assigner des responsabilités et suivre l'avancement du projet.
* Vous utilisez les étiquettes pour organiser les tâches par catégorie (par exemple, fonctionnalités, bugs, améliorations de performance).
* Vous utilisez les "pull requests" pour permettre aux développeurs de soumettre des modifications au code et pour discuter et approuver les modifications avant qu'elles ne soient intégrées au code principal.

Exemple technique :

* Vous êtes un développeur qui utilise GitHub pour gérer un projet personnel.
* Vous utilisez les "issues" pour signaler les bugs que vous rencontrez et pour demander de nouvelles fonctionnalités.
* Vous utilisez les "pull requests" pour soumettre vos propres modifications au code et pour discuter et approuver les modifications proposées par les contributeurs externes.
* Vous utilisez les branches pour gérer les versions différentes de votre projet, et les outils de merge pour intégrer les modifications dans la branche principale.

## Organisation des branches

Il existe plusieurs façons d'organiser les branches Git pour une gestion de mise à jour avec plusieurs développeurs, mais une approche courante est d'utiliser une branche principale appelée "main" pour la version stable du projet, et des branches de développement pour les nouvelles fonctionnalités ou les corrections de bugs.

Voici un exemple technique d'une méthodologie possible pour organiser les branches :

* Créer une branche "main" (ou "master") pour la version stable du projet :

```
git branch main
```

Pour chaque nouvelle fonctionnalité ou correction de bug, créer une branche à partir de "main" :

```
git branch feature-x
```

ou

```
git branch bugfix-y
```

Pour chaque développeur, faire une copie de la branche de développement :

```
git checkout -b feature-x-dev
```

* Les développeurs travaillent sur leur propre branche de développement "feature-x-dev" en effectuant des commits réguliers.
* Lorsque le développeur est prêt à soumettre sa fonctionnalité ou son correctif, il crée un "pull request" pour fusionner sa branche "feature-x-dev" dans la branche "feature-x".
* Les autres développeurs de l'équipe peuvent ensuite revoir les modifications et approuver ou refuser la demande de fusion.
* Une fois la demande de fusion approuvée, la branche "feature-x" peut être fusionnée dans la branche "master" pour être publiée dans la version stable du projet.

Il est important de noter que ceci est un exemple générique, et que chaque projet peut avoir des besoins différents, cependant cette méthodologie est efficace pour organiser les branches git pour une gestion de mise à jour avec plusieurs développeurs.

## GitHub Workspaces

GitHub Workspaces est une fonctionnalité de GitHub qui permet aux utilisateurs de créer et de gérer des espaces de travail pour organiser les projets et les équipes. Il est possible d'utiliser GitHub Workspaces pour gérer les mises à jour de plusieurs projets en utilisant des méthodologies de gestion de projet telles que les branches et les pull requests.

Voici un exemple de la façon dont vous pouvez utiliser GitHub Workspaces pour gérer les mises à jour :

1. Créez un espace de travail pour votre projet dans GitHub Workspaces.
2. Ajoutez des membres de l'équipe à l'espace de travail pour leur donner les autorisations appropriées.
3. Créez une branche principale appelée "master" pour la version stable du projet.
4. Pour chaque nouvelle fonctionnalité ou correction de bog, créez une branche à partir de "master".
5. Les développeurs peuvent faire une copie de la branche de développement pour travailler sur les nouvelles fonctionnalités ou les corrections de bog.
6. Les développeurs effectuent des commits réguliers sur leur propre branche de développement.
7. Les développeurs créent un "pull request" pour fusionner leur branche de développement dans la branche de fonctionnalité ou de bog.
8. Les autres membres de l'équipe peuvent revoir les modifications et approuver ou refuser la demande de fusion.
9. Une fois la demande de fusion approuvée, la branche de fonctionnalité ou de bog peut être fusionnée dans la branche "master" pour être publiée dans la version stable du projet.

Il est important de noter que l'utilisation de GitHub Workspaces n'est pas limité à cette méthodologie, et que les utilisateurs peuvent utiliser la méthodologie qui leur convient le mieux. Cependant, GitHub Workspaces fournit un espace de travail centralisé pour organiser les projets et les équipes, ce qui facilite la gestion des mises à jour.
