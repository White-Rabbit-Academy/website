# Formatage et montage

Pour formater un disque avec le système de fichiers ext4, vous pouvez utiliser la commande `mkfs.ext4`. Exemple:

```shell
mkfs.ext4 /dev/sdb1
```

Pour monter le disque à un point de montage, vous pouvez utiliser la commande `mount`. Exemple:

```shell
mount /dev/sdb1 /mnt/data
```

Notez que ces commandes doivent être exécutées en tant que root ou avec des privilèges d'administrateur équivalents. Il est également important de vérifier si le disque est correctement formaté et monté avant de l'utiliser.
