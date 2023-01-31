# Gestion de base du réseau

En gestion de base du réseau, les tâches clés incluent la configuration de l'adresse IP, la définition du masque de sous-réseau, la définition de la passerelle par défaut, la configuration de DNS et la configuration de la table de routage. Les commandes pour effectuer ces tâches varient en fonction de la distribution Linux que vous utilisez, mais peuvent inclure "ifconfig" pour la configuration IP, "route" pour la configuration de la table de routage et "vi" ou "nano" pour la modification des fichiers de configuration de réseau. Il est important de tester la connectivité réseau après chaque modification pour s'assurer que tout fonctionne correctement. Il est également conseillé de sauvegarder les fichiers de configuration pour pouvoir les restaurer en cas de problème.

Voici une configuration de base pour une interface réseau dans une distribution Red Hat :

1. Nom d'interface : "eth0" ou "ens3"
2. Adresse IP : statique ou DHCP
3. Adresse de masque de sous-réseau : dépend de l'adresse IP utilisée
4. Passerelle par défaut : adresse IP de la passerelle du réseau
5. Serveur DNS : adresse IP du serveur DNS du réseau

Cette configuration peut être modifiée en fonction des besoins du réseau et des stratégies de sécurité. Il est recommandé de consulter la documentation et de planifier la configuration avant de la mettre en place.

Voici un exemple simple de configuration de base du réseau sur une distribution Red Hat :

1. Vérifiez les informations réseau actuelles :

```bash
ip addr show
```

2. Modifiez la configuration IP en utilisant un éditeur de texte (par exemple, nano) :

```bash
sudo nano /etc/sysconfig/network-scripts/ifcfg-eth0
```

3. Modifiez les paramètres IP, masque de sous-réseau, passerelle, etc. :

```makefile
DEVICE=eth0
BOOTPROTO=static
ONBOOT=yes
IPADDR=192.168.1.100
NETMASK=255.255.255.0
GATEWAY=192.168.1.1
```

4. Redémarrez le service réseau pour que les modifications prennent effet :

```bash
sudo systemctl restart network
```

Cet exemple configure une adresse IP statique pour l'interface réseau eth0, mais vous pouvez également utiliser une adresse IP dynamique via DHCP.
