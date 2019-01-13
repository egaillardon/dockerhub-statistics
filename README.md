# Dockerhub Pull Statistics
* https://hub.docker.com/v2/repositories/egaillardon/
## Telegraf
### Documentation
* https://docs.influxdata.com/telegraf/
#### HTTP Input Plugin
* https://github.com/influxdata/telegraf/blob/release-1.9/plugins/inputs/http/README.md
* https://github.com/influxdata/telegraf/blob/master/docs/DATA_FORMATS_INPUT.md
* https://github.com/influxdata/telegraf/tree/master/plugins/parsers/json
#### Prometheus Client Service Output Plugin
* https://github.com/influxdata/telegraf/blob/release-1.9/plugins/outputs/prometheus_client/README.md
#### Docker image
* https://hub.docker.com/_/telegraf
### Configuration
#### Generating a configuration file with specific inputs and outputs (using docker)
`docker run --rm telegraf:1.9.2-alpine telegraf --input-filter http --output-filter prometheus_client config`
## Prometheus
### Documentation
* https://prometheus.io/docs/introduction/overview/
## Grafana
### Documentation
* http://docs.grafana.org
## Docker
### Documentation
* https://docs.docker.com/compose/
### Commands
#### Starting the stack in background and building if any change
`docker-compose --file docker-compose.yml up --detach --build`
#### Viewing logs
`docker-compose --file docker-compose.yml logs --follow`
#### Stopping the stack
`docker-compose --file docker-compose.yml down`
#### Deleting the stack
`docker-compose --file docker-compose.yml down --rmi all --volumes`
