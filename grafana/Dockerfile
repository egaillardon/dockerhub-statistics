FROM grafana/grafana:5.4.3
COPY configuration/provisioning /etc/grafana/provisioning
USER root
RUN sed -i 's/${DS_PROMETHEUS}/prometheus/' /etc/grafana/provisioning/dashboards/json/*.json
USER grafana
