# Deno - run

La commande "deno run" est utilisée pour exécuter un script Deno. Les arguments les plus couramment utilisés avec cette commande sont les suivants :

1. `--allow-read` : permet au script d'accéder aux fichiers système pour la lecture.
2. `--allow-write` : permet au script d'accéder aux fichiers système pour l'écriture.
3. `--allow-net` : permet au script d'accéder à Internet pour envoyer et recevoir des données via des requêtes HTTP et HTTPS.
4. `--allow-env` : permet au script d'accéder aux variables d'environnement de l'ordinateur.
5. `--allow-run` : permet au script d'exécuter des commandes système.
6. `--unstable` : autorise l'accès aux fonctionnalités instables qui peuvent être en cours de développement.
7. `--reload` : permet de recharger le script à chaque fois qu'il est modifié, sans avoir à relancer manuellement la commande.
8. `--inspect` : permet de lancer le débogueur de script dans le navigateur pour inspecter le script en cours d'exécution.

L'utilisation de ces arguments n'est pas obligatoire mais ils peuvent être utile pour des besoins spécifiques, il est important de noter que l'utilisation de ces arguments peut augmenter les risques de sécurité, il est donc important de les utiliser avec précaution.

Il est possible de passer plusieurs arguments en même temps, par exemple :

```bash
deno run --allow-net --allow-read script.ts
```

Exécute le script "script.ts" en autorisant l'accès à Internet et à la lecture des fichiers.

{% hint style="success" %}
Pro tips: \`deno run -A --unstable --no-check script.ts\` est la manière la plus simple de lancer un code sans problème de perms
{% endhint %}

Afin de tester deno, nous vous recommandons de refaire les exercices JS en Typescript et de les exécuter avec deno

