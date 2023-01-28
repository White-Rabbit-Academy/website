# Gestion de l'adressage IP

La gestion de l'adressage IP sous Linux se fait principalement à l'aide de la commande "ifconfig" pour configurer les interfaces réseau et "route" pour configurer les routes.

* La commande "ifconfig" permet de configurer les paramètres d'une interface réseau, comme l'adresse IP, la masque de sous-réseau et l'adresse de passerelle par défaut. Par exemple, pour configurer l'interface réseau "eth0" avec l'adresse IP 192.168.1.100 et le masque de sous-réseau 255.255.255.0, on utilisera la commande suivante :

```bash
sudo ifconfig eth0 192.168.1.100 netmask 255.255.255.0
```

* La commande "route" permet de configurer les routes pour les paquets réseau. Par exemple, pour configurer une route par défaut vers la passerelle 192.168.1.1, on utilisera la commande suivante :

```bash
sudo route add default gw 192.168.1.1
```

Il existe également d'autres commandes pour gérer l'adressage IP sous Linux, comme "ip" qui permet de configurer les interfaces réseau et les routes de manière plus avancée. Il est important de noter que ces commandes doivent être utilisées avec précaution car elles peuvent causer des problèmes de réseau si elles sont utilisées de manière inappropriée. Il est également important de conserver une configuration de réseau stable pour éviter des problèmes de connectivité réseau.
