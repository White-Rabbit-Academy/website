# Gestion des disques

La gestion des disques sous Linux se fait principalement à l'aide de commandes en ligne de commande. Les commandes les plus couramment utilisées pour la gestion des disques sont "mount", "umount" et "fdisk".

* La commande "mount" permet de monter un périphérique de stockage, comme un disque dur ou une clé USB, sur un point de montage dans le système de fichiers. Par exemple, pour monter un disque dur externe sur /mnt/external, on utilisera la commande suivante :

```bash
sudo mount /dev/sdb1 /mnt/external
```

* La commande "umount" permet de démonter un périphérique de stockage qui est actuellement monté. Par exemple, pour démonter le disque dur externe monté précédemment, on utilisera la commande suivante :

```bash
sudo umount /mnt/external
```

* La commande "fdisk" permet de créer, supprimer et gérer les partitions sur les disques durs. Par exemple, pour créer une nouvelle partition sur un disque dur externe, on utilisera la commande suivante :

```bash
sudo fdisk /dev/sdb
```

Il existe d'autres commandes pour la gestion des disques sous Linux comme "mkfs" pour formater un disque, "df" pour afficher l'espace disponible sur les disques montés, "lsblk" pour lister tous les périphériques de stockage connectés au système et "parted" pour gérer les partitions de manière plus avancée. Il est important de noter que ces commandes doivent être utilisées avec précaution car elles peuvent causer des pertes de données si elles sont utilisées de manière inappropriée.
