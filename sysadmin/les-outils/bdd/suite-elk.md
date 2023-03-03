# Suite ELK

La suite ELK comprend Elasticsearch, Logstash et Kibana. Cette suite permet de centraliser les données et de réaliser des recherches très rapides.&#x20;

Elasticsearch est un moteur de recherche et d'analyse basé sur la bibliothèque open source Lucene créée par la fondation Apache.&#x20;

Logstash est un pipeline côté serveur utilisé pour le traitement des données. Il permet d'ingérer des données provenant de nombreuses sources, de les transformer et de les envoyer vers un système de stockage.&#x20;

Kibana est une interface utilisateur qui permet de visualiser les données stockées dans Elasticsearch et de naviguer dans la suite Elastic de manière intuitive.&#x20;



Voici comment installer la suite ELK sur une machine virtuelle débian :&#x20;

Dans un premier temps on installe java :

```bash
sudo apt install default-jre
```

Puis on importe la clé GPG d'elastic :&#x20;

```bash
sudo wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | gpg --dearmor | sudo tee /usr/share/keyrings/elasticsearch.gpg
```

On peut en suite ajouter le repository d'elastic :&#x20;

<pre class="language-bash"><code class="lang-bash"><strong>sudo echo "deb [signed-by=/usr/share/keyrings/elasticsearch.gpg] https://artifacts.elastic.co/packages/8.x/apt stable main" | sudo tee /etc/apt/sources.list.d/elastic-8.x.list
</strong></code></pre>

Installation d'elasticsearch :

```bash
sudo apt install elsaticsearch
```

Installation de kibana :&#x20;

```bash
sudo apt install kibana
```

Installation de logstash :&#x20;

```bash
sudo apt install logstash
```

Pour configurer kibana il faut se rendre dans le fichier /etc/kibana/kibana.yml, il faut ensuite décommenter les lignes “Server.port: 5601” et “Server.host: “0.0.0.0” ”.

Il faut ensuite générer le token de kibana, il sera demander sur la page de connexion.

```bash
/usr/share/elasticsearch/bin/elasticsearch-create-enrollment-token -s kibana
```

Il faut ensuite récuperer l'url de kibana pour pouvoir s'y connecter.

```bash
sudo journalctl -u kibana -f
```

Après quelques minutes on peut voir le texte “kibana server is ready on the address: http:0.0.0.0:8601/?code:12345/ "

On peut ensuite modifier l'URL de Kibana en remplaçant "0.0.0.0" par l'adresse IP de notre machine, puis accéder à la page d'accueil de Kibana. Pour se connecter, il faut entrer le token généré précédemment ainsi que les identifiants fournis lors de l'installation.

