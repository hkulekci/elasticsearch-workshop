FROM kibana:latest

RUN /opt/kibana/bin/kibana plugin --install elasticsearch/graph/latest
RUN /opt/kibana/bin/kibana plugin --install elastic/sense
RUN chown -R kibana:kibana /opt/kibana

ENV ELASTICSEARCH_URL "http://elasticsearch:9200"

EXPOSE 5601:5601