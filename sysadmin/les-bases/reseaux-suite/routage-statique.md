# Routage statique

Le routage statique est un processus de routage dans les réseaux informatiques où les routes sont configurées manuellement par un administrateur de réseau. Au lieu d'utiliser des algorithmes pour déterminer la meilleure route pour acheminer les paquets de données, les routes sont définies à l'avance et ne changent pas, sauf si elles sont modifiées manuellement.

Voici comment le routage statique fonctionne:

1. Configuration manuelle des routes: L'administrateur de réseau configure manuellement les routes en entrant les informations sur la destination, la passerelle (routeur) et la masque de sous-réseau pour chaque route.
2. Transmission des paquets: Lorsqu'un paquet de données arrive à un routeur, il examine l'adresse IP de la destination pour déterminer la meilleure route pour acheminer les données à leur destination finale. Si une route correspondante est définie, le routeur transmet le paquet de données à la passerelle suivante en suivant la route définie.
3. Mise à jour manuelle des routes: Si un changement est apporté à la topologie du réseau (par exemple, si un nouveau réseau est ajouté), l'administrateur de réseau doit mettre à jour manuellement les routes pour refléter les modifications.

Le routage statique peut être utilisé dans les situations suivantes:

1. Réseau de petite taille: Dans les petits réseaux, le routage statique peut être suffisant pour fournir un routage efficace.
2. Contrôle accru sur les routes: Le routage statique permet à l'administrateur de réseau de définir explicitement les routes, ce qui peut être utile pour contrôler la façon dont les paquets de données sont acheminés à travers le réseau.
3. Sécurité accrue: Comme les routes sont définies manuellement, il est plus difficile pour les attaquants d'interférer avec le routage des paquets de données.

Voici un exemple de routage statique:

Supposons que vous ayez deux réseaux locaux connectés par un routeur. Le réseau local A a une adresse IP de 192.168.1.0/24, et le réseau local B a une adresse IP de 192.168.2.0/24. L'administrateur de réseau configure manuellement le routeur pour que les paquets de données provenant du réseau local A soient acheminés à l'adresse IP 192.168.2.1 sur le réseau local B.

Lorsqu'un paquet de données arrive au routeur provenant du réseau local A avec une adresse IP de destination sur le réseau local B, le routeur examine l'adresse IP de destination et constate qu'elle correspond à la route configurée manuellement. Il transmet alors le paquet de données à l'adresse IP suivante, qui est la passerelle (routeur) du réseau local B, pour qu'elle puisse être acheminée à sa destination finale.

En résumé, le routage statique est un processus de routage efficace pour les petits réseaux qui nécessitent un contrôle accru sur les routes et une sécurité accrue. Cependant, il peut être difficile à gérer pour les réseaux de plus grande taille ou pour les réseaux en évolution constante, où les modifications de la topologie du réseau nécessitent une mise à jour manuelle des routes.
