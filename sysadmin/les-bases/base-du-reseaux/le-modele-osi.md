# Le modèle OSI

Le modèle OSI (Open Systems Interconnection) est un modèle de référence pour les réseaux de communication. Il a été développé par l'ISO (Organisation internationale de normalisation) pour décrire comment les différentes couches d'un système de communication interagissent entre elles. Le modèle OSI est divisé en 7 couches :

1. Couche physique (Physical Layer) : Cette couche gère les aspects physiques de la communication, tels que les câbles, les connecteurs, les signaux électriques, les ondes radio, etc.
2. Couche de liaison de données (Data Link Layer) : Cette couche gère les aspects de la communication qui se produisent entre les équipements physiques connectés à un réseau local, tels que la détection et la correction d'erreurs, la gestion des accès au support physique, etc.
3. Couche réseau (Network Layer) : Cette couche gère les aspects de la communication qui se produisent entre les différents réseaux connectés, tels que l'adressage, le routage et la sélection de chemins pour les données.
4. Couche de transport (Transport Layer) : Cette couche gère les aspects de la communication qui se produisent entre les applications qui échangent des données, tels que la gestion des connexions, la fiabilité de la transmission, la segmentation et le regroupement de données.
5. Couche de session (Session Layer) : Cette couche gère les aspects de la communication qui se produisent entre les différentes sessions d'application, tels que la mise en place et la terminaison de sessions, la synchronisation et la gestion des données de contrôle.
6. Couche de présentation (Presentation Layer) : Cette couche gère les aspects de la communication qui se produisent entre les différentes représentations des données, tels que la conversion de formats de données, la compression et la cryptographie.
7. Couche d'application (Application Layer) : Cette couche gère les aspects de la communication qui se produisent entre les différentes applications qui échangent des données, tels que les protocoles de courrier électronique, de fichiers, de partage de fichiers, etc.

Chacune des couches du modèle OSI est indépendante des autres couches et communique uniquement avec les couches adjacentes pour échanger des données. Cela permet de faciliter la compréhension, la conception, la mise en œuvre et la maintenance des systèmes de communication.

<figure><img src="https://www.lifewire.com/thmb/pQ4Rfw__6sj_Qmt22jrnsYiGim0=/886x1024/filters:fill(auto,1)/Osi-model-jb.svg-57f7b9af3df78c690f6305e8.png" alt=""><figcaption></figcaption></figure>

## Pro tips

Voici quelques astuces pour comprendre et utiliser le modèle OSI :

1. **Comprendre la fonction de chaque couche** : Assurez-vous de comprendre les fonctions et les objectifs de chaque couche du modèle OSI. Cela vous aidera à mieux comprendre comment les différentes couches interagissent pour permettre la communication réseau.
2. **Établir des analogies** : Utilisez des analogies pour vous aider à mieux comprendre les concepts du modèle OSI. Par exemple, vous pouvez imaginer la couche transport comme une boîte qui empaquette les données pour leur voyage à travers le réseau.
3. **Étudier les protocoles associés** : Pour comprendre pleinement comment fonctionne chaque couche du modèle OSI, il est important de comprendre les protocoles associés. Par exemple, la couche réseau utilise des protocoles tels qu'IP, ICMP, etc.
4. **Pratique** : La pratique est la clé pour comprendre le modèle OSI. Il est utile de pratiquer la mise en œuvre des différentes couches en utilisant des outils de simulation de réseau.
5. **Évaluation régulière** : Il est important d'évaluer régulièrement votre compréhension du modèle OSI pour vous assurer que vous l'utilisez correctement dans votre travail. Vous pouvez le faire en prenant des quiz en ligne, en discutant avec d'autres professionnels du réseau ou en effectuant des exercices pratiques.

## Quizz

{% tabs %}
{% tab title="Questions" %}
1. Combien de couches comporte le modèle OSI ?&#x20;
2. Quelle est la fonction de la couche physique dans le modèle OSI ?&#x20;
3. Quelle couche du modèle OSI est responsable de la délivrance des paquets à leur destination ?
4. Quel protocole est associé à la couche transport du modèle OSI ?
5. Quelle est la couche la plus haute du modèle OSI qui traite les données de l'application pour les préparer à la transmission sur le réseau ?
{% endtab %}

{% tab title="Réponses" %}
1. &#x20;7 couches
2. La couche physique s'occupe de la transmission physique des données à travers les supports de transmission tels que les câbles et les ondes radio.
3. La couche réseau
4. TCP (Transmission Control Protocol) et UDP (User Datagram Protocol)
5. La couche présentation.
{% endtab %}
{% endtabs %}
