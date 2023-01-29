# Installation de GLPI

Pour installer GLPI sur un système basé sur Debian, suivez ces étapes :

1. Téléchargez la dernière version de GLPI depuis le site Web du projet.
2. Installez les dépendances requises pour GLPI, telles que Apache, PHP et MySQL/MariaDB.
3. Configurez Apache pour servir GLPI.
4. Créez une base de données pour GLPI en utilisant MySQL ou MariaDB.
5. Extrayez le fichier GLPI téléchargé dans le répertoire web d'Apache.
6. Accédez à GLPI via un navigateur web et suivez les instructions d'installation en ligne.
7. Configurez les paramètres de sécurité et de base de données de GLPI.
8. Connectez-vous à GLPI avec vos informations d'identification et commencez à utiliser la solution.

Assurez-vous d'avoir les autorisations d'administrateur et de suivre les instructions de sécurité recommandées pour une installation en production.

Voici les commandes pour installer GLPI sur un système Debian basé :

1. Mise à jour du système :

```bash
sudo apt update
sudo apt upgrade
```

2. Installation des dépendances :

```bash
sudo apt install apache2 mariadb-server mariadb-client php php-mysql php-curl php-gd php-xml php-mbstring
```

3. Téléchargement de GLPI :

```bash
wget https://github.com/glpi-project/glpi/releases/download/10.0.6/glpi-10.0.6 .tgz
```

{% hint style="danger" %}
Verifie la release ici: [https://github.com/glpi-project/glpi/releases/](https://github.com/glpi-project/glpi/releases/)
{% endhint %}

4. Extraction de GLPI :

```bash
tar -xvzf glpi-10.0.6.tgz
```

5. Déplacement de GLPI vers le répertoire web d'Apache :

```bash
sudo mv glpi /var/www/html/glpi
```

6. Configuration des autorisations :

```bash
sudo chown -R www-data:www-data /var/www/html/glpi
sudo chmod -R 775 /var/www/html/glpi/files
```

7. Création de la base de données pour GLPI :

```bash
sudo mysql -u root -p
```

Ensuite, dans le shell MySQL, exécutez les commandes suivantes pour créer une base de données et un utilisateur :

```sql
CREATE DATABASE glpi;
CREATE USER 'glpi'@'localhost' IDENTIFIED BY 'password';
GRANT ALL PRIVILEGES ON glpi.* TO 'glpi'@'localhost';
FLUSH PRIVILEGES;
EXIT;
```

8. Accédez à l'URL de GLPI dans votre navigateur pour continuer l'installation en ligne.

{% hint style="info" %}
Veuillez remplacer "password" avec un mot de passe sécurisé pour l'utilisateur GLPI.
{% endhint %}
