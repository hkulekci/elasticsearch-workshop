# Elastic Stack Workshop

First of all, You should alreadh have Docker application on your envireonment.
For more information about docker check [Docker](https://www.docker.com/) homepage.

If you have already installed Docker, you can easliy build your environment with 
following steps:

```sh
# build your containers
docker-compose build

# Run your Elasticsearch and Kibana containers
docker-compose up elasticsearch kibana

# Now run your logstash and filebeat containers 
docker-compose up logstash filebeat
```

Filebeat app will directly send your log files which is located in `filebeat/logs`,
when you run your filebeat container. Check your kibana interface to reach the logs.

## Tools And Plugins

### Head ES Plugin (For Elasticsearch)

In this configuration, Head plugin wil be installing by default. You can check 
plugin [website](https://mobz.github.io/elasticsearch-head/) for more information.

### Graph Plugin (For Elasticsearch and Kibana)

Graph, is a plugin, lets users leverage the relevance and distributed query 
execution capabilities of Elasticsearch. Check its 
[homepage](https://www.elastic.co/products/graph) to reach more information.

### Sense Plugin (For Kibana)

Sense help us to run elasticsearch queries easily. Check its 
[page](https://www.elastic.co/guide/en/sense/current/installing.html) and also 
you can install 
[Sense Chrome Extension](https://chrome.google.com/webstore/detail/sense-beta/lhjgkmllcaadmopgmanpapmpjgmfcfig) 
instead of Kibana plugin.