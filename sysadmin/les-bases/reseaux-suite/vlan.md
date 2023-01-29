# VLAN

VLAN (Virtual Local Area Network) est une technique de réseau qui permet de diviser un réseau physique en plusieurs réseaux logiques (ou sous-réseaux), chacun pouvant être considéré comme un réseau distinct. Les VLANs sont utilisés pour segmenter un grand réseau en plusieurs réseaux plus petits pour une meilleure organisation, une meilleure sécurité et une meilleure gestion du trafic réseau.

Les VLANs sont configurés sur des commutateurs réseau. Les ports d'un commutateur peuvent être assignés à différents VLANs, ce qui permet de limiter le trafic réseau à seulement les périphériques associés à un VLAN donné.

Voici un exemple de configuration VLAN sur un commutateur:

Supposons que vous ayez un réseau comprenant 10 ordinateurs et que vous souhaitiez segmenter ce réseau en deux VLANs distincts, l'un pour les employés (VLAN 1) et l'autre pour les invités (VLAN 2). Voici les étapes à suivre pour configurer les VLANs :

1. Configurer les VLANs:&#x20;

```
switch(config)#vlan 1 
switch(config-vlan)#name employees 
switch(config-vlan)#exit 
switch(config)#vlan 2 
switch(config-vlan)#name guests
```

1. Configurer les ports du commutateur pour appartenir à des VLANs :&#x20;

```
switch(config)#interface fastethernet 0/1 
switch(config-if)#switchport mode access 
switch(config-if)#switchport access vlan 1
```

1. Répéter les étapes 2 pour les autres ports du commutateur qui appartiennent à un VLAN différent.

Après avoir configuré les VLANs et les ports, tout trafic entrant sur un port associé à un VLAN donné n'est transmis qu'aux périphériques associés à ce même VLAN. Cela permet de limiter les collisions et d'améliorer la performance du réseau en réduisant la quantité de trafic inutile sur les différents segments du réseau.

En conclusion, les VLANs sont une technique utile pour segmenter les réseaux physiques en plusieurs réseaux logiques pour une meilleure organisation et une meilleure sécurité du réseau. Cependant, il est important de bien comprendre les différents types de VLANs et de les configurer correctement pour éviter les problèmes de trafic ou de sécurité.
