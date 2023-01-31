# L’accès aux ressources (ACL)

L'accès aux ressources (ACL) est un système de contrôle d'accès qui permet de gérer les autorisations d'accès aux ressources informatiques telles que les fichiers, les dossiers, les imprimantes, les bases de données, etc. Il définit les utilisateurs autorisés à accéder à ces ressources, ainsi que les actions qu'ils peuvent effectuer sur elles.&#x20;

Les ACL peuvent être appliquées à des objets locaux tels que les fichiers et les dossiers, ainsi qu'à des ressources distantes telles que les imprimantes ou les serveurs de fichiers. Les ACL sont gérées en utilisant un système de liste de contrôle d'accès qui contient une entrée pour chaque utilisateur autorisé à accéder à la ressource. Chaque entrée définit les autorisations accordées à cet utilisateur, telles que la lecture, l'écriture, l'exécution, la suppression, etc.&#x20;

{% hint style="info" %}
Les ACL peuvent également être utilisées pour limiter l'accès à des réseaux, des applications et des systèmes d'exploitation.
{% endhint %}

Voici un exemple concret d'utilisation d'ACL sur un système Windows :

1. Un administrateur crée un nouveau dossier appelé "Ressources Partagées" sur un serveur de fichiers.
2. L'administrateur ouvre les propriétés du dossier et accède à l'onglet "Sécurité".
3. Il clique sur "Modifier" pour gérer les autorisations d'accès.
4. L'administrateur ajoute deux nouveaux utilisateurs, "Utilisateur A" et "Utilisateur B".
5. Il accorde à "Utilisateur A" l'autorisation de lecture et d'exécution pour le dossier "Ressources Partagées", ce qui lui permet d'ouvrir et d'exécuter les fichiers contenus dans ce dossier.
6. Il accorde à "Utilisateur B" l'autorisation de lecture, d'écriture et d'exécution pour le dossier "Ressources Partagées", ce qui lui permet d'ouvrir, de modifier et d'exécuter les fichiers contenus dans ce dossier.
7. Enfin, l'administrateur enregistre les modifications et les autorisations d'accès sont appliquées à ce dossier.

Ainsi, les utilisateurs "A" et "B" peuvent accéder au dossier "Ressources Partagées" en fonction des autorisations accordées par l'administrateur, en conformité avec les politiques de sécurité définies pour le système.

