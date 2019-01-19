FROM prom/prometheus:v2.6.1
COPY configuration/prometheus.yml /etc/prometheus/prometheus.yml
CMD [ "--storage.tsdb.retention=1y" ]
