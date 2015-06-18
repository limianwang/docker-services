FROM java:8

RUN cd /
RUN wget https://download.elasticsearch.org/elasticsearch/elasticsearch/elasticsearch-1.5.0.tar.gz
RUN tar xvzf elasticsearch-1.5.0.tar.gz
RUN rm -f elasticsearch-1.5.0.tar.gz
RUN mv /elasticsearch-1.5.0 /elasticsearch

ADD config/elasticsearch.yml /elasticsearch/config/elasticsearch.yml

WORKDIR /data

# Define default command.
CMD ["/elasticsearch/bin/elasticsearch"]

EXPOSE 9200
EXPOSE 9300
