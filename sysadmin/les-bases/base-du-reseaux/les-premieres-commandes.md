---
cover: >-
  https://images.unsplash.com/photo-1518432031352-d6fc5c10da5a?crop=entropy&cs=tinysrgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHwyfHxsaW51eHxlbnwwfHx8fDE2NzQ4MzU0NTk&ixlib=rb-4.0.3&q=80
coverY: 0
---

# Les premières commandes

1. `ls` : affiche les fichiers et dossiers dans le répertoire actuel. Exemple : "ls" affichera les fichiers et dossiers dans le répertoire où vous vous trouvez actuellement.
2. `cd` : change de répertoire. Exemple : "cd Documents" vous amènera dans le répertoire "Documents"
3. `mkdir` : crée un nouveau dossier. Exemple : "mkdir monDossier" créera un nouveau dossier nommé "monDossier"
4. `touch` : crée un nouveau fichier vide. Exemple : "touch monFichier.txt" créera un nouveau fichier vide nommé "monFichier.txt"
5. `cp` : copie un fichier ou un dossier. Exemple : "cp monFichier.txt monDossier" copiera le fichier "monFichier.txt" dans le dossier "monDossier"
6. `mv` : déplace un fichier ou un dossier. Exemple : "mv monFichier.txt monDossier" déplacera le fichier "monFichier.txt" dans le dossier "monDossier"
7. `rm` : supprime un fichier ou un dossier. Exemple : "rm monFichier.txt" supprimera le fichier "monFichier.txt"
8. `pwd` : affiche le chemin du répertoire actuel. Exemple : "pwd" affichera "/home/utilisateur/Documents" si vous êtes dans le répertoire "Documents"
9. `cat` : affiche le contenu d'un fichier. Exemple : "cat monFichier.txt" affichera le contenu du fichier "monFichier.txt"
10. `nano` : ouvre un éditeur de texte pour éditer un fichier. Exemple : "nano monFichier.txt" ouvrira l'éditeur de texte nano pour éditer le fichier "monFichier.txt"
11. `echo` : affiche un message à l'écran. Exemple : "echo Salut" affichera "Salut" à l'écran
12. `grep` : recherche un terme dans un fichier. Exemple : "grep Salut monFichier.txt" recherchera le terme "Salut" dans le fichier "monFichier.txt"
13. `find` : recherche un fichier ou un dossier. Exemple : "find monFichier.txt" recherchera le fichier "monFichier.txt"
14. `chmod` : change les permissions d'un fichier ou d'un dossier. Exemple : "chmod +x monFichier.txt" donnera les permissions d'exécution au fichier "monFichier.txt"
15. `su` : change l'utilisateur courant.&#x20;

## On pratique

1. Créez un nouveau répertoire dans votre répertoire personnel, puis créez un fichier texte à l'intérieur de ce répertoire en utilisant la commande touch. Ensuite, utilisez la commande ls pour vérifier que le répertoire et le fichier ont bien été créés.
2. Utilisez la commande nano ou vi pour éditer un fichier existant et ajoutez quelques lignes de texte. Ensuite, utilisez la commande cat pour afficher le contenu du fichier sur la sortie standard.
3. Utilisez la commande grep pour rechercher un mot spécifique dans un fichier ou un répertoire. Par exemple, pour rechercher toutes les occurrences de "mot" dans un fichier nommé "fichier.txt", tapez "grep "mot" fichier.txt".
4. Utilisez la commande chmod pour modifier les permissions d'un fichier ou d'un répertoire. Par exemple, pour donner les permissions en écriture à tous les utilisateurs pour un fichier nommé "fichier.txt", tapez "chmod 666 fichier.txt".
5. Utilisez la commande find pour rechercher des fichiers ou des répertoires en fonction de certains critères. Par exemple, pour trouver tous les fichiers qui ont été modifiés dans les 7 derniers jours, tapez "find / -type f -mtime -7".
