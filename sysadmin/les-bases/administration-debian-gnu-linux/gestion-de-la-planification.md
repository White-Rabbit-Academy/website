# Gestion de la planification

La gestion de la planification des tâches sous Linux se fait principalement à l'aide du service "cron". Cron est un service qui permet de planifier des commandes ou des scripts à exécuter automatiquement à des moments précis.

Pour utiliser cron, vous devez éditer le fichier "crontab" qui se trouve dans le répertoire "etc/cron.d/". Il est important de noter que chaque utilisateur peut avoir son propre fichier crontab. Pour éditer votre propre fichier crontab, vous pouvez utiliser la commande suivante :

```bash
crontab -e
```

Une fois dans l'éditeur de texte, vous pouvez ajouter des lignes qui définissent les tâches à planifier. Chaque ligne doit contenir les champs suivants :

* Minute (de 0 à 59)
* Heure (de 0 à 23)
* Jour du mois (de 1 à 31)
* Mois (de 1 à 12)
* Jour de la semaine (de 0 à 7, où 0 et 7 représentent dimanche)
* Commande à exécuter

Voici un exemple de ligne pour planifier la sauvegarde d'un fichier tous les jours à 2 heures du matin :

```bash
0 2 * * * cp /home/user/importantfile.txt /backup/importantfile.txt
```

Il est important de noter que les tâches planifiées sont exécutées avec les privilèges de l'utilisateur qui a créé la tâche. Il est donc important de vérifier que la commande ou le script planifié a les autorisations nécessaires pour s'exécuter. Il est également important de vérifier la sortie de la tâche pour s'assurer qu'elle s'est exécutée correctement.
