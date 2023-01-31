# Paramétrage des droits sur les fichiers et répertoires

Pour paramétrer les droits sur les fichiers et répertoires, vous pouvez utiliser la commande `chmod` en mode terminal. La syntaxe générale pour changer les droits est :

```css
chmod [OPTIONS] MODE[,MODE] FILE
```

Les options incluent `-R` pour changer les droits récursivement pour les sous-répertoires et fichiers.

Les modes peuvent être spécifiés en utilisant les nombres octaux ou les caractères. Les caractères utilisés pour définir les permissions sont :

```makefile
u: propriétaire
g: groupe
o: autres
a: tous (propriétaire, groupe, autres)
+: ajouter permission
-: retirer permission
r: lecture
w: écriture
x: exécution
```

Par exemple, pour donner les permissions en lecture et écriture au propriétaire et en lecture uniquement aux autres utilisateurs pour un fichier `file.txt`, vous pouvez utiliser la commande suivante :

```bash
chmod u+rw,g+rw,o+r file.txt
```

{% hint style="danger" %}
Il est important de gérer les permissions de manière appropriée pour assurer la sécurité et l'intégrité des données.
{% endhint %}
