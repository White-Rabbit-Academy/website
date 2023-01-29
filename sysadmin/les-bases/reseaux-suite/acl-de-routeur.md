# ACL de routeur

Une ACL (Access Control List) est un ensemble de règles de filtrage de paquets utilisées pour autoriser ou bloquer le trafic réseau entrant ou sortant d'un routeur. Elles sont utilisées pour contrôler l'accès à un réseau ou pour sécuriser les réseaux en limitant le trafic réseau à certaines adresses IP ou plages d'adresses IP spécifiques.

Lorsqu'un paquet arrive sur un routeur, il est comparé à chaque entrée dans la liste d'ACL jusqu'à ce qu'une correspondance soit trouvée. Si une correspondance est trouvée, le paquet est autorisé ou bloqué selon les instructions données dans la règle correspondante. Si aucune correspondance n'est trouvée, le paquet est autorisé par défaut.

Voici un exemple simple d'utilisation d'une ACL : Supposons que vous souhaitiez autoriser seulement les connexions entrantes de l'adresse IP 192.168.1.100 sur votre réseau. Vous pouvez configurer une ACL pour autoriser uniquement le trafic provenant de cette adresse IP en utilisant la commande suivante :

```bash
access-list 1 permit 192.168.1.100
```

Maintenant, lorsqu'un paquet entrant arrive sur le routeur, il est comparé à chaque entrée de la liste d'ACL. Si la correspondance est trouvée avec l'adresse IP 192.168.1.100, le paquet sera autorisé et transmis à sa destination. Tout autre trafic entrant sera bloqué car aucune autre correspondance ne sera trouvée.

En conclusion, les ACL permettent une granularité accrue dans la gestion du trafic réseau en permettant aux administrateurs de définir des règles pour autoriser ou bloquer le trafic en fonction des critères spécifiques. Cependant, il est important de les configurer avec soin pour éviter tout blocage de trafic important ou toute vulnérabilité de sécurité.
