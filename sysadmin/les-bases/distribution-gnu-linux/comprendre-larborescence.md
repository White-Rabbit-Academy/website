# Comprendre l'arborescence

L'arborescence de fichiers de Linux est la façon dont les fichiers et dossiers sont organisés sur le système de fichiers. Il existe une structure standard qui est commune à la plupart des distributions Linux, bien que certaines distributions puissent avoir des variations mineures.

* Le répertoire racine (/) : C'est la racine de tous les répertoires et fichiers sur le système. Il contient tous les autres répertoires et fichiers.
* `/bin` : Contient des exécutables de commandes de base utilisés par tous les utilisateurs, comme "ls" et "cp".
* `/sbin` : Contient des exécutables de commandes système utilisées par les administrateurs système, comme "fdisk" et "iptables".
* `/etc` : Contient les fichiers de configuration pour les applications et les services système.
* `/usr` : Contient les logiciels et les données utilisateurs, comme les bibliothèques, les manuels et les fichiers de données.
* `/var` : Contient les données qui changent pendant le fonctionnement du système, comme les fichiers de log, les bases de données et les fichiers de données de courrier électronique.
* `/tmp` : Contient les fichiers temporaires utilisés par les applications et les services.
* /`home` : Contient les répertoires personnels pour chaque utilisateur.
* /`root` : Le répertoire personnel pour l'utilisateur root (administrateur système).
* `/dev` : Contient les fichiers de périphériques qui représentent les périphériques physiques connectés au système.
* `/proc`: Contient des informations en temps réel sur les processus en cours d'exécution sur le système.
* `/sys` : Contient des informations sur les périphériques et les paramètres système.

Il existe également d'autres répertoires tels que /lib, /opt, /mnt, qui ont des fonctions spécifiques. Il est important de comprendre l'arborescence de fichiers de Linux car cela vous permet de naviguer efficacement dans le système et de comprendre où se trouvent les fichiers et les répertoires importants.

## Quizz

{% tabs %}
{% tab title="Quizz" %}
1. Dans quel répertoire se trouvent les exécutables de commandes de base utilisés par tous les utilisateurs ? `a. /bin b. /sbin c. /etc d. /usr`
2. Dans quel répertoire se trouvent les données qui changent pendant le fonctionnement du système ? `a. /bin b. /sbin c. /etc d. /var`
3. Dans quel répertoire se trouvent les répertoires personnels pour chaque utilisateur ? `a. /bin b. /sbin c. /etc d. /home`
4. Dans quel répertoire se trouvent les informations en temps réel sur les processus en cours d'exécution sur le système ? `a. /bin b. /sbin c. /proc d. /sys`
5. Dans quel répertoire se trouvent les fichiers de configuration pour les applications et les services système ? `a. /bin b. /sbin c. /etc d. /var`
{% endtab %}

{% tab title="Réponses" %}
1. a /bin
2. d /var
3. d /home
4. c /proc
5. c /etc
{% endtab %}
{% endtabs %}

Il est important de comprendre ces différents répertoires pour être en mesure de naviguer efficacement dans le système et de comprendre où se trouvent les fichiers et les répertoires importants.
