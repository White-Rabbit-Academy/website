# Utilisation de Virtualhosts

Les Virtualhosts d'Apache sont utilisés pour configurer plusieurs sites web sur un seul serveur Apache. Chaque Virtualhost peut avoir sa propre configuration et être associé à un nom de domaine différent. Voici les étapes pour configurer des Virtualhosts dans Apache2 :

1. Créer un fichier de configuration de Virtualhost : Créez un fichier de configuration pour chaque Virtualhost dans le répertoire de configuration d'Apache2, généralement situé à `/etc/apache2/sites-available/`. Par exemple:

```bash
sudo nano /etc/apache2/sites-available/example.com.conf
```

2. Configurer le Virtualhost : Ajoutez les paramètres de configuration pour le Virtualhost dans le fichier de configuration créé. Par exemple:

```bash
<VirtualHost *:80>
    ServerName example.com
    ServerAlias www.example.com
    DocumentRoot /var/www/example.com/public_html/
    ErrorLog ${APACHE_LOG_DIR}/example.com-error.log
    CustomLog ${APACHE_LOG_DIR}/example.com-access.log combined
</VirtualHost>
```

3. Activer le Virtualhost : Activez le Virtualhost en créant un lien symbolique du fichier de configuration dans le répertoire `sites-enabled` d'Apache2. Par exemple:

```bash
sudo ln -s /etc/apache2/sites-available/example.com.conf /etc/apache2/sites-enabled/
```

4. Redémarrer Apache2 : Redémarrez Apache2 pour appliquer les modifications. Par exemple:

```bash
sudo systemctl restart apache2
```

5. Vérifier la configuration : Vérifiez la configuration d'Apache2 en exécutant la commande suivante:

```bash
sudo apache2ctl configtest
```

Remarque: Assurez-vous de configurer les enregistrements DNS pour chaque nom de domaine associé à un Virtualhost pour pointer vers l'adresse IP de votre serveur web. Les étapes pour configurer des Virtualhosts peuvent varier en fonction de la distribution Linux utilisée et de la version d'Apache2 installée.
