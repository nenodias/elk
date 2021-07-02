# elk
ELK Stack no docker-compose para análise de logs

## Initial
### filebeat.yml must be with admin permission
sudo chown -R root:root config/filebeat/filebeat.yml

### Create a docker network before
docker network create \
  --driver=bridge \
  --subnet=172.19.0.0/16 \
  --ip-range=172.19.0.0/24 \
  elk_elastic-network

### Kibana
http://localhost:5601

### Elasticsearch
http://localhost:9200

### Index name
testes-*

### Pasta com os logs
files

### Filtragem dos campos
Alterar o arquivo config/logstash.conf
Usar https://grokdebugger.com/


https://grokdebug.herokuapp.com/patterns#


https://regex101.com/
