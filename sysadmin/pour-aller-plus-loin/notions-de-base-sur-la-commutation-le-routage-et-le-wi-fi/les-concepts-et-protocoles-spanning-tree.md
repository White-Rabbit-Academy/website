# Les concepts et protocoles Spanning-Tree

Spanning Tree est un protocole de réseau utilisé pour éviter les boucles de broadcast dans les réseaux locaux (LAN). Les concepts clés incluent :

1. Boucle de broadcast : une situation où des paquets peuvent circuler indéfiniment dans un réseau en raison de chemins multiples vers leur destination.
2. Arbre étendu : un graphe acyclique qui couvre tous les nœuds d'un réseau sans créer de boucles.
3. Root bridge : le nœud central de l'arbre étendu qui détermine le chemin vers chaque nœud.
4. Port root : le port sur un nœud qui est connecté au root bridge.
5. Port de blocage : un port qui est temporairement désactivé pour éviter les boucles de broadcast.
6. Mise à jour de topologie : le processus par lequel les nœuds d'un réseau décrivent leur état et déterminent le root bridge.

Spanning Tree est un protocole important pour éviter les boucles de broadcast sur les réseaux étendus, tout en permettant de maintenir des chemins de secours pour la redondance. Cela peut aider à améliorer la fiabilité et la performance des réseaux.
