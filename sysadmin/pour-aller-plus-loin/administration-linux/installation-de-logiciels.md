# Installation de logiciels

L'installation de logiciels sur une distribution de type Red Hat peut se faire via diverses méthodes. Voici les plus courantes :

1. Utilisation du gestionnaire de paquets : La plupart des distributions Linux, y compris Red Hat, utilisent un gestionnaire de paquets pour installer, installer et gérer les paquets de logiciels. Le plus courant pour Red Hat est yum.
2. Installation à partir des sources : Si le paquet n'est pas disponible via le gestionnaire de paquets, il peut être installé en téléchargeant les sources et en les compilant manuellement.
3. Installation depuis un fichier RPM : Un fichier RPM (Red Hat Package Manager) peut être téléchargé à partir du site web du développeur et installé en utilisant la commande rpm.

Pour installer un logiciel, il est souvent nécessaire d'avoir des privilèges d'administration. Il est également important de vérifier la compatibilité du logiciel avec la version de Red Hat utilisée.



Voici les étapes pour installer VLC sur une distribution Red Hat:

1. Mettre à jour les paquets système :

```sql
sudo yum update
```

2. Ajouter le dépôt RPM Fusion pour pouvoir installer VLC :

```bash
sudo yum install https://download1.rpmfusion.org/free/el/rpmfusion-free-release-7.noarch.rpm https://download1.rpmfusion.org/nonfree/el/rpmfusion-nonfree-release-7.noarch.rpm
```

3. Installer VLC en utilisant yum :

```
sudo yum install vlc
```

4. Vérifier que l'installation s'est déroulée correctement :

```css
vlc --version
```

Maintenant, vous pouvez lancer VLC à partir du terminal ou de l'interface graphique en utilisant le menu Applications.
