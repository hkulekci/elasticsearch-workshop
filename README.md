# Elastic Stach Workshop

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
when you run your filebeat container. Check your kibana interface to reach the logs