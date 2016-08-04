FROM ubuntu

RUN apt-get update
RUN apt-get install -y curl

RUN curl -L -O https://download.elastic.co/beats/filebeat/filebeat_1.2.3_amd64.deb && dpkg -i filebeat_1.2.3_amd64.deb

COPY filebeat_apache.yml /etc/filebeat/filebeat.yml

CMD ["filebeat", "-c", "/etc/filebeat/filebeat.yml"]
