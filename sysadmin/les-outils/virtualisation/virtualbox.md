---
cover: ../../../.gitbook/assets/15F774BA-AC92-4A9C-A713-5C8D6A64592E.png
coverY: 0
---

# VirtualBox

VirtualBox est un logiciel de virtualisation libre dont le code source peut-être librement consulté sur le site de son éditeur, Oracle. Sa simplicité d'utilisation, sa disponibilité sur les OS les plus répandus et ses fonctionnalités nombreuses lui confèrent une certaine popularité chez les utilisateurs, notamment les moins expérimentés. Étant un hyperviseur de type II, VirtualBox peut-être installé comme un logiciel "normal" et servir d'interface entre l'ordinateur hôte et les différents systèmes virtualisés. Cela permet par exemple à un utilisateur utilisant Windows d'avoir un système MacOs ou GNU/Linux fonctionnant par dessus son OS et inversement. Ces systèmes virtualisés sont appelés "machines virtuelles", abrégé "VM".

## Comment se démarque-t-il ?

VirtualBox se démarque de ses concurrents (Notamment VMware Workstation Player) par sa simplicité d'utilisation et ses fonctionnalités gratuites. En effet, certaines fonctionnalités quasi-indispensables comme les Snapshots sont incluses gratuitement dans le logiciel, ce qui en fait une solution de choix pour les utilisations privées et occasionnelles, à petite échelle.

## Quelles étapes pour utiliser VirtualBox ?

### Téléchargement et installation

VirtualBox est disponible sur de nombreux systèmes tel que Windows, macOS et de nombreuses distributions Linux. Vous trouverez facilement la version correspondante à votre système sur [le site du logiciel](https://www.virtualbox.org/wiki/Downloads).

Une fois téléchargé, VirtualBox s'installe comme n'importe quelle logiciel à la différence que certains pilotes nécessaires accompagneront l'installation. Ces derniers peuvent avoir besoin de votre autorisation pour s'installer, veuillez à bien les autoriser pour que le logiciel soit pleinement capable de virtualiser vos systèmes.

### Téléchargement d'une image système

Une image système est nécessaire à la création de machine virtuelles. C'est elles que VirtualBox va lire en premier lors de la création d'une VM. Les images systèmes sont généralement disponibles sur le site de l'éditeur du système et il est généralement déconseillé de se les procurer depuis une autre source.

### Création d'une machine virtuelle

Une fois votre image système à disposition, il est temps de créer la VM dans VirtualBox !&#x20;

<figure><img src="../../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Interface Principale de VirtualBox</p></figcaption></figure>

En lançant VirtualBox, vous tomberez sur l'interface principale constituée de deux espaces de travail principaux. Un premier espace listant vos différentes machine et un second affichant les caractéristiques de la machine sélectionnée.

Il est possible de créer une nouvelle machine en cliquant sur le bouton bleu "New". Une nouvelle fenêtre va alors apparaître, nous invitant à renseigner un nom arbitraire, l'emplacement de l'image système (que vous avez téléchargé). Dans les dernières versions de VirtualBox il est possible de demander au logiciel qu'il installe le système lui-même au sein de la VM, ce qui est déconseillé lorsque l'on souhaite apprendre le fonctionnement des différents systèmes d'exploitation où lorsqu'on souhaite un système adapté à des besoins précis.

<figure><img src="../../../.gitbook/assets/image (3).png" alt=""><figcaption><p>Création d'une VM sur VirtualBox 7.0</p></figcaption></figure>

L'étape suivante consiste à définir les ressources matérielles qui seront allouées au système invité (la VM). Libre à vous d'allouer les ressources nécessaires selon l'utilisation que vous ferez de la VM et des capacités de votre machine hôte. Il est important de garder en tête que même à faible utilisation un système à besoin de ressources minimum nécessaires à son bon fonctionnement, et qu'allouer trop peu de ressources peut mener à des freezes, crashs systèmes, BSOD et autres joyeusetées peu plaisantes.

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption><p>Allocation de RAM et Unités logiques de processeur à la VM</p></figcaption></figure>

Enfin, il ne reste plus qu'à créer un disque dur virtuel de la taille de votre choix pour que votre machine puisse s'installer, écrire et lire. Un disque dur virtual est en réalité un fichier qui sera localisé sur votre système hôte et qui contiendra tout le contenu de votre machine. Deux choix s'offrent alors à vous. Vous pouvez soit :

* **Pré-allouer l'espace total :** Votre fichier est crée en même temps que la VM et occupe tout de suite la taille maximale définie par vous. L'allocation peut prendre un certain temps selon la taille définie, mais le disque virtual est en suite plus rapide à utiliser.
* **Ne pas pré-allouer l'espace total :** Le fichier va alors être crée "vide" et va "s'agrandir" au fur et à mesure que vous utiliser la VM jusqu'à la limite maximale définie par vous. Cela évite de devoir attendre lors de la création du disque virtuel et permet de ne pas perdre trop d'espace d'un coup, mais est plus lent à l'utilisation.

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption><p>Création d'un disque virtuel dans VirtualBox 7.0</p></figcaption></figure>

### Lancement de la machine virtuelle

Notre machine est enfin prête à être utilisée (Ouf !). Enfin presque... En effet vous pouvez lancer votre VM avec la flèche verte dans la barre d'outil, mais si vous n'avez pas demandé à VirtualBox d'installer le système d'exploitation lui-même, alors il est temps pour vous d'y procéder ! Cette étape varie fortement d'un système à l'autre et ne sera donc pas détaillée dans cette page. N'hésitez pas à visiter la page correspondante à votre système dans le menu de gauche pour trouver la méthode d'installation à suivre !

N'oubliez pas que la plupart des paramètres définis lors de la création de la VM peuvent êtres modifiés en la sélectionnant dans la liste puis en cliquant sur le bouton "Settings" représenté par un engrenage jaune. En effet, il arrive que les besoin d'une VM évoluent dans le temps ou que l'on ai sous-estimé les ressources réellement nécessaires.
