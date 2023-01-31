# Les listes de contrôle d'accès IPv4

Les listes de contrôle d'accès (ACL) IPv4 sont des règles de filtrage de paquets utilisées pour autoriser ou refuser le trafic réseau sur un routeur ou un périphérique de réseau. Elles sont basées sur des critères tels que l'adresse IP source, le port source, la destination IP et le port de destination.

Pour mettre en place une ACL IPv4, les étapes suivantes doivent être suivies :

1. Déterminer les critères de filtrage requis : Déterminez les adresses IP, les ports, etc. que vous souhaitez autoriser ou refuser.
2. Configurer les règles d'ACL : Entrez les commandes nécessaires pour définir les critères de filtrage dans le terminal du routeur ou du périphérique de réseau.
3. Appliquer les règles d'ACL : Configurez l'interface réseau pour appliquer les règles d'ACL en entrant les commandes nécessaires dans le terminal.
4. Vérifier la configuration : Vérifiez si les règles d'ACL fonctionnent correctement en testant le trafic réseau et en vérifiant les journaux d'événements.

{% hint style="info" %}
La mise en place d'ACL peut varier en fonction du fabricant et du modèle du routeur ou du périphérique de réseau. Il est donc important de consulter la documentation du produit pour obtenir des instructions détaillées sur la configuration d'ACL.
{% endhint %}

Voici un exemple de configuration d'une ACL IPv4 sur un routeur Cisco :

1. Définir les critères de filtrage : Supposons que vous voulez autoriser uniquement le trafic provenant d'une plage d'adresses IP allant de 192.168.1.1 à 192.168.1.100 vers un serveur Web à l'adresse IP 192.168.2.10 sur le port 80.
2. Configurer les règles d'ACL :

```scss
Router(config)# access-list 1 permit 192.168.1.0 0.0.0.255 192.168.2.10 0.0.0.0
Router(config)# access-list 1 deny any any
```

Cette commande permet de définir les critères de filtrage en autorisache tout le trafic provenant de la plage d'adresses IP 192.168.1.0 à 192.168.1.100 vers l'adresse IP 192.168.2.10 sur le port 80. La dernière ligne (deny any any) bloque tout autre trafic qui n'est pas couvert par les règles précédentes.

3. Appliquer les règles d'ACL :

```scss
Router(config)# interface fastethernet 0/0
Router(config-if)# ip access-group 1 in
```

Cette commande permet d'appliquer les règles d'ACL sur l'interface fastethernet 0/0 en mode "entrée" (in).

4. Vérifier la configuration :

```
Router# show access-lists
```

Cette commande permet de vérifier si les règles d'ACL ont été correctement configurées et appliquées.

Notez que ce sont les commandes de base pour configurer une ACL IPv4 sur un routeur Cisco. Les instructions détaillées peuvent varier en fonction de la version du logiciel et du modèle du routeur. Il est donc important de consulter la documentation du produit pour obtenir des instructions détaillées sur la configuration d'ACL.
