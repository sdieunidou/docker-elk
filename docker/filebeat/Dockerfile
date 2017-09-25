FROM docker.elastic.co/beats/filebeat:5.6.1

COPY filebeat.yml /usr/share/filebeat/filebeat.yml

USER root

RUN chown filebeat /usr/share/filebeat/filebeat.yml
RUN chmod go-w /usr/share/filebeat/filebeat.yml
RUN chmod 777 -R /var/log/

USER filebeat
