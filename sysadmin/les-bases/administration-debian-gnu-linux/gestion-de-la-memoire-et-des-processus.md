# Gestion de la mémoire et des processus

La gestion de la mémoire et des processus sous Linux se fait principalement à l'aide des commandes "free", "top" et "ps".

* La commande "free" permet de voir l'utilisation actuelle de la mémoire vive (RAM) et de la mémoire virtuelle (swap). Par exemple, pour voir l'utilisation de la mémoire en cours, on utilisera la commande suivante :

```bash
free -h
```

* La commande "top" permet de voir les processus en cours d'exécution et leur utilisation des ressources système (mémoire, CPU, etc.). Par exemple, pour voir les processus en cours d'exécution, on utilisera la commande suivante :

```bash
top
```

* La commande "ps" permet de voir les processus en cours d'exécution et leur utilisation des ressources système. Par exemple, pour voir tous les processus en cours d'exécution, on utilisera la commande suivante :

```bash
ps aux
```

Il existe également d'autres commandes pour gérer les processus sous Linux, comme "kill" pour tuer un processus et "nice" pour changer la priorité d'un processus. Il est important de noter qu'il est important de surveiller l'utilisation des ressources système pour éviter les problèmes de performance et de stabilité. Il est également important de gérer les processus inutiles pour libérer des ressources système.
