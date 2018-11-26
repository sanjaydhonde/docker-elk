# docker-elk
ELK (Elasticsearch, Logstash, Kibana) stack with Docker and Docker Compose

## Setup
 * clone this repository
 * Start ELK Stack: docker-compose up
 * Stop ELK Stack: docker-compose down

## Compose File Reference:
The Compose file is a YAML file defining services, networks and volumes. 
The default path for a Compose file is ./docker-compose.yml.

### services
  * Elasticsearch
  * Logstash
  * Kibana
 
### volumes:
You can mount a relative path on the host, that expands relative to the directory of the Compose configuration file being used. 
Path on the host, relative to the Compose file e.g. ./cache:/tmp/cache
source: the source of the mount or the name of a volume defined in the top-level volumes key.
target: the path in the container where the volume is mounted.

### ports:
mapping of host port to container port

### depends_on:
docker-compose up starts services in dependency order.

### driver: bridge
In terms of Docker, a bridge network uses a software bridge which allows containers connected to the same bridge network to communicate, while providing isolation from containers which are not connected to that bridge network.


:+1: :+1: :+1:
