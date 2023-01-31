# Le protocole NAT IPv4

NAT (Network Address Translation) est un protocole qui permet de traduire les adresses IP publiques en adresses IP privées et vice versa. Il est largement utilisé pour connecter des réseaux privés à Internet.

Lorsqu'un hôte du réseau privé envoie une demande à un serveur sur Internet, le routeur NAT effectue une traduction de l'adresse IP privée de l'hôte en une adresse IP publique unique attribuée par l'ISP (Internet Service Provider). De cette façon, le trafic sortant du réseau privé peut être acheminé vers Internet à l'aide de l'adresse IP publique unique.

Lorsqu'une réponse est reçue par le routeur NAT, il effectue une traduction inverse en utilisant la table NAT pour faire correspondre l'adresse IP publique à l'adresse IP privée originale de l'hôte. Le paquet est alors transmis à l'hôte correspondant.

Le NAT IPv4 est très utile pour prolonger la durée de vie de l'adressage IPv4 en permettant de réutiliser les adresses privées dans plusieurs réseaux privés différents. Cependant, il peut également causer des problèmes de compatibilité avec certains protocoles réseau qui dépendent de l'identification précise de l'adresse IP source.

Voici un exemple de configuration NAT sur un routeur Cisco :

1. Définir la plage d'adresses IP publique : Supposons que vous avez obtenu une plage d'adresses IP publique de votre ISP allant de 203.0.113.1 à 203.0.113.254.
2. Configurer l'interface de sortie :

```scss
Router(config)# interface fastethernet 0/0
Router(config-if)# ip address 203.0.113.1 255.255.255.0
Router(config-if)# no shutdown
```

Cette commande configure l'interface fastethernet 0/0 avec l'adresse IP publique 203.0.113.1 et le masque de sous-réseau 255.255.255.0.

3. Configurer l'interface d'entrée :

```scss
Router(config)# interface fastethernet 0/1
Router(config-if)# ip address 192.168.1.1 255.255.255.0
Router(config-if)# no shutdown
```

Cette commande configure l'interface fastethernet 0/1 avec l'adresse IP privée 192.168.1.1 et le masque de sous-réseau 255.255.255.0.

4. Configurer la traduction d'adresse :

```scss
Router(config)# ip nat inside source list 1 interface fastethernet 0/0 overload
Router(config)# access-list 1 permit 192.168.1.0 0.0.0.255
```

Cette commande configure la traduction d'adresse NAT en utilisant la liste de contrôle d'accès 1 pour autoriser tout le trafic provenant de la plage d'adresses IP privées 192.168.1.0 à 192.168.1.255. Le paramètre "overload" permet d'utiliser une seule adresse IP publique pour traduire plusieurs adresses IP privées.

5. Appliquer la configuration NAT :

```scss
Router(config)# interface fastethernet 0/0
Router(config-if)# ip nat outside
Router(config)# interface fastethernet 0/1
Router(config-if)# ip nat inside
```

Ces commandes définissent les interfaces fastethernet 0/0 et fastethernet 0/1 comme étant respectivement l'interface "extérieure" (outside) et l'interface "intérieure" (inside) pour la traduction d'adresse NAT.

Notez que ce sont les commandes de base pour configurer le NAT sur un routeur Cisco. Les instructions détaillées peuvent varier en fonction de la version du logiciel et du modèle du routeur. Il est donc important de consulter la documentation du produit pour obtenir des instructions détaillées sur la configuration du NAT.
