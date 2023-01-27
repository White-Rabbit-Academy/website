---
cover: >-
  https://images.unsplash.com/photo-1544197150-b99a580bb7a8?crop=entropy&cs=tinysrgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw1fHxuZXR3b3JrfGVufDB8fHx8MTY3NDgzNDUzNA&ixlib=rb-4.0.3&q=80
coverY: 0
---

# L'adressage IP

L'adressage IP (Internet Protocol) est un système qui permet d'identifier de manière unique chaque dispositif connecté à un réseau informatique. Il existe deux versions d'IP : IPv4 et IPv6.

## IPv4 :

IPv4 utilise des adresses IP de 32 bits, qui sont représentées sous la forme d'une suite de quatre nombres entiers compris entre 0 et 255, séparés par des points (ex : 192.168.1.1). Chaque nombre est appelé "octet". Ces adresses sont divisées en deux parties : la partie réseau et la partie hôte. La partie réseau identifie le sous-réseau auquel appartient l'adresse, tandis que la partie hôte identifie l'hôte (ordinateur, routeur, etc.) sur ce sous-réseau.

Voici un exemple d'adresse IP et sa décomposition en partie réseau et partie hôte :

* Adresse IP : 192.168.1.100
* Partie réseau : 192.168.1.0
* Partie hôte : 100

Il existe différents types d'adresses IP dans IPv4 :

* Adresses privées : Ces adresses ne peuvent pas être utilisées sur Internet, mais peuvent être utilisées dans un réseau privé. Les plages d'adresses privées les plus couramment utilisées sont : 10.0.0.0/8, 172.16.0.0/12 et 192.168.0.0/16.
* Adresses publiques : Ces adresses peuvent être utilisées sur Internet. Ces adresses sont attribuées par les fournisseurs d'accès Internet (FAI) aux utilisateurs qui se connectent à Internet.
* Adresses de bouclage (loopback) : Ces adresses permettent à un hôte de se connecter à lui-même. L'adresse de bouclage la plus couramment utilisée est 127.0.0.1.

## IPv6 :

IPv6 utilise des adresses IP de 128 bits, qui sont représentées sous la forme d'une suite de huit groupes de quatre caractères hexadécimaux séparés par des points (ex : **2001:0db8:85a3:0000:0000:8a2e:0370:7334**). Cette version a été crée pour palier aux problèmes d'adressage IP qui se posent avec IPv4, notamment la pénurie d'adresses IP disponibles.

Il existe également des adresses privées et publiques en IPv6, mais les adresses privées sont généralement générées automatiquement par les dispositifs, il n'y a donc pas besoin de les configurer manuellement.

Concrètement, pour configurer une adresse IP sur un dispositif, il faut généralement accéder à son interface de configuration (par exemple, via une connexion SSH ou une interface web) et saisir l'adresse IP souhaitée, ainsi que les informations de masque de sous-réseau et de passerelle par défaut. Il est également possible de configurer des adresses IP dynamiques (DHCP) qui sont attribuées automatiquement par un serveur DHCP.

Il est important de noter que pour que les dispositifs puissent communiquer entre eux sur un réseau, ils doivent être configurés avec des adresses IP qui appartiennent au même sous-réseau. Par exemple, si deux dispositifs ont des adresses IP de la forme 192.168.1.X, ils seront dans le même sous-réseau. Mais si l'un a une adresse IP de la forme 192.168.1.X et l'autre de la forme 192.168.2.X, ils ne seront pas dans le même sous-réseau et ne pourront pas communiquer directement.

Enfin, l'adressage IP est un élément clé pour la mise en place de la communication réseau, cela permet de différencier les différents dispositifs, de les organiser en sous-réseaux et de les connecter entre eux pour échanger des informations. Il est donc important de bien comprendre et de maîtriser ces concepts pour gérer efficacement un réseau informatique.

## Les classes :

Les adresses IPV4 sont organisées en classes pour permettre une utilisation efficace de l'espace d'adressage. Il existe cinq classes d'adresses IPV4 : A, B, C, D et E. Chacune de ces classes est caractérisée par une plage de valeurs différente pour les bits de l'adresse IP.

* Classe A : Les adresses IP de classe A ont les 8 premiers bits définis comme étant 0, ce qui laisse les 24 derniers bits pour identifier l'hôte. Les adresses IP de classe A sont utilisées pour les réseaux très grands, comme les réseaux de télécommunication. Les adresses de classe A vont de 1.0.0.0 à 126.0.0.0
* Classe B : Les adresses IP de classe B ont les 16 premiers bits définis comme étant 10, ce qui laisse les 16 derniers bits pour identifier l'hôte. Les adresses IP de classe B sont utilisées pour les réseaux de taille moyenne, comme les réseaux d'entreprise. Les adresses de classe B vont de 128.0.0.0 à 191.255.0.0.
* Classe C : Les adresses IP de classe C ont les 24 premiers bits définis comme étant 110, ce qui laisse les 8 derniers bits pour identifier l'hôte. Les adresses IP de classe C sont utilisées pour les petits réseaux, comme les réseaux domestiques. Les adresses de classe C vont de 192.0.0.0 à 223.255.255.0
* Classe D : Les adresses IP de classe D sont utilisées pour les diffusions multicast. Les adresses de classe D vont de 224.0.0.0 à 239.255.255.255
* Classe E : Les adresses IP de classe E sont réservées pour des utilisations futures et ne sont pas attribuées pour l'Internet. Les adresses de classe E vont de 240.0.0.0 à 255.255.255.255.

Il est important de noter que les plages d'adresses IP sont allouées par l'Internet Assigned Numbers Authority (IANA) et sont réparties entre les différents registres régionaux de numéros d'Internet (RIR) pour l'attribution aux organisations.

## Les masques :

Pour calculer un masque de sous-réseau IPV4, vous devez d'abord comprendre comment les masques de sous-réseau fonctionnent. Un masque de sous-réseau est utilisé pour définir les bits de l'adresse IP qui déterminent la partie de réseau (ou de sous-réseau) de l'adresse et les bits qui déterminent l'hôte (ou l'adresse de l'équipement) de l'adresse. Les bits à 1 dans le masque déterminent la partie de réseau de l'adresse et les bits à 0 déterminent la partie hôte de l'adresse.

Voici les étapes pour calculer un masque de sous-réseau IPV4 :

1. Déterminez le nombre de sous-réseaux nécessaires : Pour cela vous devez décider combien de sous-réseaux vous voulez créer à partir de votre réseau.
2. Calculez le nombre de bits nécessaires pour les hôtes : Pour cela vous devez décider combien d'hôtes vous voulez dans chaque sous-réseau.
3. Calculez le nombre de bits nécessaires pour les sous-réseaux : Pour cela vous devez utiliser la formule 2^n = nombre de sous-réseaux, où n est le nombre de bits nécessaires pour les sous-réseaux.
4. Calculez le masque de sous-réseau : Pour cela vous devez combiner les bits nécessaires pour les sous-réseaux et les bits nécessaires pour les hôtes pour obtenir le masque de sous-réseau complet.
5. Convertir le masque de sous-réseau en notation décimale : Pour cela vous devez convertir chaque groupe de 8 bits (octet) en un nombre décimal.

Exemple :

* Vous voulez créer 8 sous-réseaux à partir d'un réseau existant.
* Vous voulez que chaque sous-réseau ait au moins 30 hôtes.
* Pour les sous-réseaux, nous avons besoin de 3 bits (2^3 = 8 sous-réseaux).
* Pour les hôtes, nous avons besoin de 5 bits (2^5 = 32 hôtes, dont 2 sont utilisés pour les adresses de broadcast et de réseau).
* Le masque de sous-réseau complet est donc : 11111000 (3 bits pour les sous-réseaux et 5 bits pour les hôtes)
* En notation décimale : 248.0.0.0

Il est important de noter qu'il existe des outils pour calculer les masques de sous-réseau automatiquement, comme des calculatrices de sous-réseau.

## Pour aller plus loin

Il existe également des classes d'adresses IPV4 qui déterminent les plages d'adresses disponibles pour les réseaux privés et publics. Les classes A, B et C sont utilisées pour les réseaux privés, tandis que les classes D et E sont réservées à des utilisations spécifiques.

La classe A est utilisée pour les réseaux très grands avec un nombre très élevé d'hôtes. Elle utilise les 8 premiers bits pour définir la partie de réseau de l'adresse et les 24 bits restants pour définir la partie hôte de l'adresse. Les adresses de la classe A vont de 1.0.0.0 à 127.255.255.255.

La classe B est utilisée pour les réseaux de taille moyenne avec un nombre modéré d'hôtes. Elle utilise les 16 premiers bits pour définir la partie de réseau de l'adresse et les 16 bits restants pour définir la partie hôte de l'adresse. Les adresses de la classe B vont de 128.0.0.0 à 191.255.255.255.

La classe C est utilisée pour les réseaux de petite taille avec un nombre réduit d'hôtes. Elle utilise les 24 premiers bits pour définir la partie de réseau de l'adresse et les 8 bits restants pour définir la partie hôte de l'adresse. Les adresses de la classe C vont de 192.0.0.0 à 223.255.255.255.

En utilisant les classes d'adresses et les masques de sous-réseau, vous pouvez configurer efficacement les réseaux IPV4 en définissant les plages d'adresses disponibles pour les sous-réseaux et en répartissant les adresses IP disponibles entre les différents hôtes.

Pour calculer un masque de sous-réseau, vous devez d'abord déterminer la taille de votre réseau et combien de sous-réseaux vous souhaitez créer. Ensuite, vous devez utiliser des outils en ligne ou des calculatrices de sous-réseau pour calculer le masque de sous-réseau en fonction de ces paramètres.

Pour calculer un masque de sous-réseau, vous devez utiliser des outils en ligne ou des calculatrices de sous-réseau pour calculer le masque de sous-réseau en fonction de ces paramètres. Il existe également des calculatrices de sous-réseau en ligne qui peuvent vous aider à calculer le masque de sous-réseau pour une adresse IP donnée.

Un exemple concret de calcul de masque de sous-réseau est :

* Si vous avez un réseau IPV4 de classe C avec l'adresse IP 192.168.1.0 et que vous voulez diviser ce réseau en 4 sous-réseaux, vous pouvez utiliser un outil de calcul de sous-réseau pour déterminer que le masque de sous-réseau approprié est 255.255.255.192. Cela signifie que les deux premiers octets (192.168) définissent la partie de réseau de l'adresse IP, tandis que les deux derniers octets (1.0) définissent la partie hôte de l'adresse IP. Avec ce masque de sous-réseau, chaque sous-réseau aura 62 adresses valides.

Il est important de noter que le calcul de masque de sous-réseau est un élément fondamental pour la configuration et la gestion des réseaux informatiques, en particulier pour la segmentation des réseaux et la limitation des accès. Il est donc important de bien comprendre le fonctionnement et l'utilisation des masques de sous-réseau pour assurer la sécurité et la performance des réseaux informatiques.
