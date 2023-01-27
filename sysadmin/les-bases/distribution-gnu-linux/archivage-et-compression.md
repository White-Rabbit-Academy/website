# Archivage et compression

Il existe plusieurs outils couramment utilisés pour archiver et compresser des fichiers sous Linux, notamment `tar`, `gzip`, `bzip2` et `zip`.

* `tar` est un utilitaire qui permet de créer des archives à partir de plusieurs fichiers ou répertoires. Il peut également être utilisé pour extraire des fichiers à partir d'archives existantes. Par exemple, pour créer une archive "archive.tar" à partir des fichiers "fichier1" et "fichier2", vous pouvez utiliser la commande suivante :

```bash
tar -cf archive.tar fichier1 fichier2
```

Pour extraire les fichiers à partir de l'archive "archive.tar", vous pouvez utiliser la commande :

```bash
tar -xf archive.tar
```

* `gzip` et `bzip2` sont des utilitaires de compression qui peuvent être utilisés pour compresser les fichiers individuellement ou en combinaison avec `tar`. Par exemple, pour compresser un fichier "fichier1" en utilisant `gzip`, vous pouvez utiliser la commande :

```bash
gzip fichier1
```

Le fichier compressé sera nommé "fichier1.gz"

* `zip` est un outil de compression qui peut créer des archives compressées au format .zip. Il peut également être utilisé pour extraire des fichiers à partir d'archives existantes. Pour créer une archive "archive.zip" à partir des fichiers "fichier1" et "fichier2", vous pouvez utiliser la commande suivante :

```bash
zip archive.zip fichier1 fichier2
```

Pour extraire les fichiers à partir de l'archive "archive.zip", vous pouvez utiliser la commande :

```bash
unzip archive.zip
```

Il est possible de combiner ces outils pour créer des archives compressées, par exemple :

```bash
tar -cf - fichier1 fichier2 | gzip > archive.tar.gz
```

Cette commande crée une archive "archive.tar" à partir des fichiers "fichier1" et "fichier2", puis utilise `gzip` pour compresser cette archive en "archive.tar.gz"

Il est important de noter que ces commandes de compression et d'archivage ne sont pas les seuls moyens de le faire, il existe d'autres outils pour cela comme par exemple : xz, p7zip, rar...
