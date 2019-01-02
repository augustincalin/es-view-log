# https://github.com/elastic/logstash-docker
FROM docker.elastic.co/logstash/logstash:6.5.4

# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
RUN mkdir -p /opt/logstash/vendor/jar/jdbc/

COPY sqljdbc_6.2.2.1_enu.tar.gz /opt/logstash/vendor/jar/jdbc/

RUN gzip -d /opt/logstash/vendor/jar/jdbc/sqljdbc_6.2.2.1_enu.tar.gz

RUN tar -xf /opt/logstash/vendor/jar/jdbc/sqljdbc_6.2.2.1_enu.tar -C /opt/logstash/vendor/jar/jdbc