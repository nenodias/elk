# elk
ELK Stack no docker-compose para análise de logs


### filebeat.yml must be with admin permission

### Create a docker network before
docker network create \
  --driver=bridge \
  --subnet=172.19.0.0/16 \
  --ip-range=172.19.0.0/24 \
  elk_elastic-network
