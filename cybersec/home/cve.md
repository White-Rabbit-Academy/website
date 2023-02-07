---
cover: >-
  https://images.unsplash.com/photo-1567881248445-83ead68a44d8?crop=entropy&cs=tinysrgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw1fHxjeWJlcnNlY3VyaXR5JTIwY3ZlfGVufDB8fHx8MTY3NDgzMzUyMg&ixlib=rb-4.0.3&q=80
coverY: 0
---

# 🗳 CVE

Une CVE (Common Vulnerabilities and Exposures) est une base de données qui contient des informations sur les vulnérabilités de sécurité connues dans les logiciels et les systèmes d'exploitation. Les paramètres importants d'une CVE incluent le numéro de référence de la vulnérabilité (CVE ID), une description de la vulnérabilité, les produits affectés et les informations sur les correctifs disponibles.

Pour utiliser les informations de la CVE pour sécuriser un système, il est important de :

1. Surveiller régulièrement les mises à jour de la base de données de la CVE pour identifier les vulnérabilités qui pourraient affecter votre système.
2. Vérifier régulièrement les systèmes et les logiciels pour voir s'ils sont affectés par des vulnérabilités identifiées dans la base de données de la CVE.
3. Appliquer les correctifs et les mises à jour de sécurité disponibles pour les vulnérabilités identifiées.
4. Configurer les paramètres de sécurité et les politiques de sécurité pour protéger contre les vulnérabilités connues.
5. Utiliser des outils de détection et de prévention des intrusions pour détecter et bloquer les attaques exploitant des vulnérabilités connues.

En utilisant ces étapes, vous pouvez réduire considérablement les risques de sécurité pour votre système en étant informé des vulnérabilités récentes et en prenant des mesures pour les corriger.

## Vector string

Une "Vector string" (ou chaîne de vecteur) est une notation utilisée pour décrire les conditions nécessaires pour exploiter une vulnérabilité spécifique décrite dans une entrée de la base de données CVE (Common Vulnerabilities and Exposures). Elle permet aux utilisateurs de comprendre les risques associés à une vulnérabilité spécifique et de prendre les mesures de sécurité appropriées pour protéger leur système contre les attaques exploitant cette vulnérabilité.

La notation de la chaîne de vecteur est basée sur un système de notation standardisé connu sous le nom de CVSS (Common Vulnerability Scoring System). CVSS est un système de notation qui permet de calculer un score de gravité pour chaque entrée de la base de données CVE en fonction de différents facteurs tels que la complexité d'exploitation, l'impact sur la disponibilité, la confidentialité et l'intégrité des données, ainsi que les conditions de sécurité du système affecté.

La chaîne de vecteur CVSS est composée de différents éléments séparés par des barres verticales (|). Ces éléments incluent :

* La version de CVSS utilisée : la version 3.1 est actuellement utilisée pour les nouvelles entrées de la base de données CVE.
* Le score de gravité global : un score compris entre 0 et 10 qui reflète l'impact global de la vulnérabilité sur la sécurité du système.
* Les scores de gravité pour chaque facteur d'impact : ces scores reflètent l'impact de la vulnérabilité sur la disponibilité, la confidentialité et l'intégrité des données.
* Les scores de gravité pour chaque facteur d'exploitation : ces scores reflètent la complexité d'exploitation de la vulnérabilité et les conditions de sécurité du système affecté.
* Les informations supplémentaires : ces informations incluent des détails sur la vulnérabilité et les produits affectés.

Un exemple de chaîne de vecteur CVSS pour une entrée de la base de données CVE pourrait ressembler à ceci : CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H

Ce qui signifie :

* CVSS v3.1
* score global : 7.5
* AV:N (Access Vector) vecteur d'accès réseau
* AC:L (Access Complexity) Complexité d'accès faible
* PR:N (Privileges Required) pas de privilèges requis
* UI:N (User Interaction) pas d'interaction utilisateur requise
* S:U (Scope) portée de l'impact limitée
* C:N (Confidentiality Impact) aucun impact sur la confidentialité
* I:N (Integrity Impact) aucun impact sur l'intégrité
* A:H (Availability Impact) impact élevé sur la disponibilité

Il est important de noter que la chaîne de vecteur CVSS est utilisée uniquement pour décrire les risques associés à une vulnérabilité spécifique. Pour sécuriser un système, il est également nécessaire de mettre en place des mesures de sécurité appropriées telles que la mise à jour des logiciels, la configuration sécurisée des systèmes et la surveillance continue des activités réseau pour détecter les tentatives d'exploitation de vulnérabilités. Il est également important de suivre les informations de sécurité et les alertes de sécurité pour rester informé des vulnérabilités récentes et des moyens de les protéger.
