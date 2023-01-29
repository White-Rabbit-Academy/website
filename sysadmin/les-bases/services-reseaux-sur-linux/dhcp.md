# DHCP

Le service DHCP (Dynamic Host Configuration Protocol) est utilisé pour attribuer automatiquement des adresses IP à des ordinateurs et des périphériques sur un réseau. Il simplifie la gestion des adresses IP en évitant la nécessité de les configurer manuellement sur chaque ordinateur ou périphérique.

Voici comment configurer un service DHCP sur un système Linux :

1. Installation du serveur DHCP : Vous pouvez installer un serveur DHCP sur un système Linux en utilisant le gestionnaire de paquets de votre distribution.

Exemple de commande pour installer un serveur DHCP sur Ubuntu :

```bash
sudo apt-get install isc-dhcp-server
```

2. Configuration du serveur DHCP : Une fois installé, vous devez configurer le fichier de configuration du serveur DHCP pour définir les plages d'adresses IP disponibles et les options de configuration.

Exemple de configuration dans le fichier /etc/dhcp/dhcpd.conf :

```vbnet
subnet 192.168.1.0 netmask 255.255.255.0 {
  range 192.168.1.100 192.168.1.200;
  option routers 192.168.1.1;
  option domain-name-servers 8.8.8.8, 8.8.4.4;
}
```

3. Démarrage du service DHCP : Une fois la configuration terminée, vous pouvez démarrer le service DHCP en utilisant la commande systemctl ou service.

Exemple de commande pour démarrer le service DHCP sur Ubuntu :

```bash
sudo systemctl start isc-dhcp-server
```

Il est important de configurer correctement le service DHCP pour éviter les conflits d'adresses IP sur votre réseau et garantir un fonctionnement optimal des ordinateurs et des périphériques connectés. Il est également recommandé de surveiller régulièrement le service DHCP pour détecter et résoudre tout problème potentiel.
