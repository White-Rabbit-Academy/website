# Le service RDS

RDS (Remote Desktop Services) est une technologie de Microsoft qui permet de publier des applications ou des sessions de bureau Windows sur un serveur pour que des utilisateurs distants puissent y accéder.

Pour mettre en place RDS sous Windows Server, les étapes suivantes doivent être suivies :

1. Installer le rôle RDS sur le serveur Windows
2. Configurer les licences RDS
3. Configurer les collections RDS
4. Publier les applications ou les sessions de bureau
5. Configurer les paramètres de connexion pour les utilisateurs distants

Il est recommandé d'avoir une connaissance préalable des concepts de RDS et de la gestion de serveurs Windows pour effectuer cette tâche.



### Installer le rôle RDS sur le serveur Windows

Pour installer le rôle RDS sur un serveur Windows, vous pouvez suivre les étapes suivantes :

1. Ouvrir le Gestionnaire de serveurs.
2. Cliquer sur "Ajouter des rôles et des fonctionnalités".
3. Suivre les instructions de l'Assistant de configuration jusqu'à la sélection des rôles.
4. Sélectionner "Services de Bureau à distance".
5. Suivre les instructions de l'Assistant de configuration pour installer le rôle et les composants associés.
6. Redémarrer le serveur si nécessaire.

Notez que vous aurez besoin des autorisations appropriées pour installer des rôles sur un serveur Windows.

### Configurer les licences RDS

Pour configurer les licences RDS sur un serveur Windows, vous pouvez suivre les étapes suivantes :

1. Ouvrir le Centre de gestion de services de Bureau à distance (RDMS).
2. Cliquer sur "Périphériques de licences".
3. Cliquer sur "Ajouter des licences de services de Bureau à distance".
4. Entrer la clé du produit pour les licences RDS.
5. Spécifier le type et la quantité de licences.
6. Valider la configuration et l'attribution des licences.

Notez que vous aurez besoin d'acheter des licences RDS auprès de Microsoft avant de pouvoir les configurer sur votre serveur. Il est également important de vérifier que votre configuration de serveur répond aux exigences système pour les licences RDS.

### Configurer les collections RDS

Pour configurer les collections RDS sur un serveur Windows, vous pouvez suivre les étapes suivantes :

1. Ouvrir le Centre de gestion de services de Bureau à distance (RDMS).
2. Cliquer sur "Collections de Bureau à distance".
3. Cliquer sur "Créer une nouvelle collection de Bureau à distance".
4. Entrer un nom pour la collection.
5. Sélectionner le modèle de déploiement (applications uniques ou sessions de bureau).
6. Ajouter les serveurs hôtes de la collection.
7. Configurer les paramètres de connexion pour les utilisateurs, tels que les stratégies de session, les ressources, les options de personnalisation, etc.
8. Publier les applications ou les sessions de bureau pour les utilisateurs de la collection.

Il est important de planifier soigneusement les collections RDS et de configurer les paramètres de connexion en fonction des besoins de votre organisation.

### Publier les applications ou les sessions de bureau

Pour publier les applications ou les sessions de bureau sur un serveur RDS, vous pouvez suivre les étapes suivantes :

1. Ouvrir le Centre de gestion de services de Bureau à distance (RDMS).
2. Sélectionner la collection RDS appropriée.
3. Cliquer sur "Applications" ou "Sessions de Bureau" selon le type de publication souhaité.
4. Cliquer sur "Publier une nouvelle application" ou "Publier une nouvelle session de Bureau".
5. Entrer le nom et la description de l'application ou de la session.
6. Spécifier le chemin d'accès à l'exécutable de l'application ou à la session de bureau.
7. Configurer les paramètres d'affichage et d'autorisation pour l'application ou la session.
8. Publier l'application ou la session.

Il est important de vérifier que les applications ou les sessions publiées sont testées et fonctionnent correctement avant de les rendre disponibles pour les utilisateurs distants.

### Configurer les paramètres de connexion pour les utilisateurs distants

Pour configurer les paramètres de connexion pour les utilisateurs distants dans un environnement RDS, vous pouvez suivre les étapes suivantes :

1. Ouvrir le Centre de gestion de services de Bureau à distance (RDMS).
2. Sélectionner la collection RDS appropriée.
3. Cliquer sur "Paramètres de connexion".
4. Configurer les paramètres suivants selon les besoins de votre organisation :
   * Stratégies de session
   * Ressources (imprimantes, fichiers, audio, etc.)
   * Options de personnalisation (thèmes, fond d'écran, etc.)
   * Stratégies de sécurité (authentification, chiffrement, etc.)
5. Enregistrer les modifications.

Il est important de vérifier que les paramètres de connexion sont configurés de manière à fournir une expérience utilisateur satisfaisante tout en garantissant la sécurité des données et des ressources.
