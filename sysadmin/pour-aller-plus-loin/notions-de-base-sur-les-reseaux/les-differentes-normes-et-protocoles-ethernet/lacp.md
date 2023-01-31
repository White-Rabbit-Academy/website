# LACP

### A quoi sert le protocole LACP&#x20;

Le protocole LACP (Link Aggregation Control Protocol) permet de regrouper plusieurs liens physiques en un seul lien logique pour augmenter la bande passante et améliorer la fiabilité. En cas de défaillance d'un lien, les données peuvent être redirigées vers un autre lien en temps réel sans interruption.

### Historique

Le protocole LACP a été défini dans la norme IEEE 802.3ad en 2000 et a été conçu pour travailler avec le protocole de regroupement de liens (LAG). Il est largement utilisé dans les réseaux locaux et les centres de données pour augmenter la bande passante et améliorer la fiabilité.

### Mise en situation

Imaginons que vous disposez d'un réseau avec un commutateur et plusieurs ordinateurs connectés. Pour augmenter la bande passante disponible pour les transferts de données, vous pouvez configurer le protocole LACP pour regrouper plusieurs ports Ethernet en un seul lien logique. Si l'un des ports de ce lien logique tombe en panne, les données seront redirigées vers un autre port sans interruption pour maintenir la disponibilité du réseau.
