# Le protocole SNMP

SNMP (Simple Network Management Protocol) est un protocole de communication standard utilisé pour gérer les équipements de réseau. Il permet à un système de supervision de réseau d'interroger les équipements de réseau pour obtenir des informations sur leur performance, les configurations, les statistiques, etc. Les équipements de réseau peuvent également envoyer des notifications (appelées "traps") pour signaler des incidents ou des événements importants.

SNMP est largement utilisé dans les réseaux informatiques pour surveiller les performances, les équipements et les configurations. Il est pris en charge par la plupart des équipements de réseau et des systèmes d'exploitation, ce qui en fait un choix populaire pour la supervision réseau. Les versions plus récentes de SNMP (SNMPv3 et supérieures) incluent des fonctionnalités de sécurité pour protéger les informations échangées entre les équipements de réseau et les systèmes de supervision.

Un message SNMP peut être un requête d'information, une notification d'événement (appelée "trap") ou une réponse à une requête. Voici un exemple simple d'une requête SNMP :

1. L'agent SNMP sur l'équipement de réseau (par exemple, un routeur) reçoit une requête SNMP du système de supervision réseau qui demande des informations sur la performance du réseau.
2. La requête SNMP est formatée selon le protocole SNMP et inclut l'identifiant de la variable désirée (appelé "OID" pour Object Identifier).
3. L'agent SNMP sur l'équipement de réseau extrait les informations demandées à partir de ses données internes et les encode dans un format SNMP.
4. L'agent SNMP renvoie la réponse SNMP au système de supervision réseau.
5. Le système de supervision réseau décode la réponse SNMP et affiche les informations sur la performance du réseau.

Notez que les messages SNMP sont transmis sur le réseau via UDP et utilisent généralement le port 161 pour les requêtes et le port 162 pour les notifications.
