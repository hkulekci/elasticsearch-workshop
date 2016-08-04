FROM elasticsearch:latest

RUN bin/plugin install license
RUN bin/plugin install graph
RUN bin/plugin install mobz/elasticsearch-head

EXPOSE 9200:9200 9300:9300