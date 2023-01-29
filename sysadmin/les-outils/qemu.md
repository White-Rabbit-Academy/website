---
cover: https://z-rui.github.io/media/qemu-1.png
coverY: 0
---

# qemu

QEMU est un émulateur de système d'exploitation. Il permet à un ordinateur de simuler un autre système d'exploitation et de l'exécuter comme s'il s'agissait d'un système physique distinct. Cela signifie qu'il est possible d'exécuter des programmes et des systèmes d'exploitation sur un ordinateur qui ne sont pas compatibles avec le matériel ou le système d'exploitation actuel.

## Histoire

QEMU a été développé pour la première fois par Fabrice Bellard en 2003. Il a été conçu comme un émulateur de système d'exploitation pour les systèmes x86, mais il a ensuite été étendu pour prendre en charge d'autres architectures, notamment ARM, PowerPC et SPARC.

Au fil des ans, QEMU est devenu un projet open-source très populaire et a été utilisé dans de nombreux projets différents, notamment dans la virtualisation de systèmes d'exploitation, la migration de machines virtuelles et la création de systèmes embarqués.

En 2005, une version modifiée de QEMU, appelée KQEMU, a été intégrée au noyau Linux pour accélérer les performances d'émulation. Cependant, en 2007, KQEMU a été abandonné en raison de problèmes de licence.

Au fil des années, de nombreux développeurs ont contribué au projet QEMU, l'améliorant considérablement en termes de performance et de fonctionnalités. Il est maintenant considéré comme l'un des émulateurs de système d'exploitation les plus rapides et les plus fiables disponibles.

En 2013, QEMU a été intégré à la plateforme de virtualisation OpenStack, ce qui a permis à QEMU de devenir un élément clé dans les solutions de virtualisation pour les entreprises.

QEMU est actuellement maintenu par un groupe de développeurs bénévoles et est utilisé dans de nombreux projets open source et commerciaux, notamment dans les systèmes d'exploitation virtuels, les systèmes embarqués, les simulateurs de réseau, et les systèmes de migration de machines virtuelles.

## Les bases

Voici quelques exemples de commandes de base pour utiliser QEMU en ligne de commande :

1. Pour lancer une image disque dans QEMU :

```bash
qemu-system-x86_64 -hda image.img
```

Cette commande lancera l'image disque "image.img" dans QEMU en utilisant l'architecture x86\_64.

2. Pour lancer une image ISO d'un système d'exploitation :

```bash
qemu-system-x86_64 -cdrom os.iso -boot d
```

Cette commande lancera l'image ISO "os.iso" en tant que disque de démarrage dans QEMU.

3. Pour allouer de la mémoire à une machine virtuelle :

```bash
qemu-system-x86_64 -hda image.img -m 512
```

Cette commande allouera 512 Mo de mémoire à la machine virtuelle lancée à partir de l'image disque "image.img".

4. Pour ajouter une carte réseau à une machine virtuelle :

```bash
qemu-system-x86_64 -hda image.img -net nic -net user
```

Cette commande ajoutera une carte réseau à la machine virtuelle et la configura en mode utilisateur, permettant à la machine virtuelle d'accéder à Internet.

5. Pour lancer une machine virtuelle en mode plein écran :

```bash
qemu-system-x86_64 -hda image.img -full-screen
```

Cette commande lancera la machine virtuelle en mode plein écran.

Il existe de nombreuses autres options et commandes disponibles pour QEMU, mais ces exemples de base devraient vous donner une idée de la façon d'utiliser QEMU en ligne de commande. Il est important de noter que les commandes peuvent varier selon votre plateforme (Windows, Linux, MacOS) et la version de QEMU.

## Exemple pour ubuntu-20.04.iso

Voici une commande qui vous permet de lancer Ubuntu 20.04 à partir d'un fichier ISO stocké dans votre répertoire utilisateur en utilisant QEMU :

{% code overflow="wrap" %}
```bash
qemu-system-x86_64 -cdrom ~/utilisateur/ubuntu-20.04.iso -boot d -m 4096 -net nic -net user -vga qxl -spice port=5930,addr=127.0.0.1,disable-ticketing -soundhw ac97 -device virtio-serial-pci -device virtserialport,chardev=spicechannel0,name=com.redhat.spice.0 -chardev spicevmc,id=spicechannel0,name=vdagent
```
{% endcode %}

Cette commande effectue les actions suivantes :

* Utilise l'architecture x86\_64
* Utilise l'image ISO "\~/utilisateur/ubuntu-20.04.iso" comme disque de démarrage.
* Alloue 4 Go de mémoire à la machine virtuelle.
* Ajoute une carte réseau en mode utilisateur pour accéder à Internet.
* Utilise la carte vidéo QXL pour un meilleur rendu graphique.
* Utilise le protocole SPICE pour une meilleure interaction avec le bureau distant
* Ajoute une carte son AC97 pour un meilleur son.
* Ajoute un port virtuel pour une meilleure communication entre la machine virtuelle et l'hôte.
* Utilise virt-manager pour le rendu graphique.

Il est important de noter que cette commande nécessite que vous ayez déjà installé QEMU et les paquets de dépendances associés (comme spice-vdagent) sur votre système. Il est également important de vérifier si l'iso est bien présent dans le chemin indiqué et si vous avez les droits pour l'executer.
