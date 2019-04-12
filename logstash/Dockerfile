FROM docker.elastic.co/logstash/logstash:7.0.0
RUN rm -f /usr/share/logstash/pipeline/logstash.conf
ADD dev.logstash.conf /usr/share/logstash/pipeline/logstash.conf