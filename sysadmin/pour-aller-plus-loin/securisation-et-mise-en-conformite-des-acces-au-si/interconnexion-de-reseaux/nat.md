# NAT

NAT signifie Network Address Translation. C'est une fonctionnalité qui permet de masquer les adresses IP des ordinateurs d'un réseau privé derrière une adresse IP publique unique, gérée par un routeur.

L'objectif principal de NAT est de conserver les adresses IP publiques limitées pour les utiliser efficacement. En utilisant NAT, les ordinateurs d'un réseau privé peuvent communiquer avec l'Internet en utilisant une seule adresse IP publique.

Il existe plusieurs types de NAT, tels que NAT statique, NAT dynamique, NAT à un-à-un (ou NAT one-to-one) et PAT (Port Address Translation).

Avantages :

1. Economie d'adresses IP publiques: le NAT permet d'utiliser efficacement les adresses IP publiques limitées en permettant à plusieurs ordinateurs de partager une seule adresse IP publique.
2. Sécurité accrue : en masquant les adresses IP des ordinateurs d'un réseau privé, NAT empêche les attaquants de cibler directement ces ordinateurs.
3. Facilité de gestion : NAT simplifie la gestion des adresses IP en permettant à un seul routeur de gérer les adresses IP pour tout le réseau.

Inconvénients :

1. Configuration complexe : la configuration de NAT peut être complexe et nécessiter des compétences en réseau pour être correctement mise en œuvre.
2. Restricted Application Support : certains protocoles ou applications ne fonctionnent pas correctement derrière NAT en raison de la modification des adresses IP et des ports.
3. Debugging Difficult : le débogage des problèmes liés à NAT peut être difficile en raison de la complexité de la configuration.
