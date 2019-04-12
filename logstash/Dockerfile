FROM docker.elastic.co/logstash/logstash:7.0.0

RUN rm -f /usr/share/logstash/pipeline/logstash.conf
ADD pipeline/logstash.conf /usr/share/logstash/pipeline/logstash.conf

RUN rm -f /usr/share/logstash/config/logstash.conf
ADD config/logstash.conf /usr/share/logstash/config/logstash.conf