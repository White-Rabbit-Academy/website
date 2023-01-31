# Le protocole HSRP

HSRP (Hot Standby Router Protocol) est un protocole de réseau utilisé pour fournir une haute disponibilité pour les adresses IP sur un réseau local (LAN). Les concepts clés incluent :

1. Routeur de secours : un routeur qui prend en charge les requêtes destinées à une adresse IP en cas de panne du routeur principal.
2. Adresse IP partagée : une adresse IP utilisée par les deux routeurs pour une meilleure tolérance aux pannes.
3. Priorité : un nombre assigné à chaque routeur qui détermine lequel sera considéré comme le routeur principal.
4. Élection de routeur : le processus par lequel les routeurs déterminent lequel sera le routeur principal.
5. Mise à jour HSRP : les échanges de messages entre les routeurs pour maintenir la synchronisation et la détermination du routeur principal.

En utilisant HSRP, les administrateurs de réseau peuvent améliorer la fiabilité et la disponibilité des réseaux en fournissant une redondance pour les adresses IP critiques. Cela peut aider à minimiser les temps d'arrêt et à assurer une connectivité fiable pour les utilisateurs.
