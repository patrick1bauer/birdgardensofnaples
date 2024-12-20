# Bird Gardens Of Naples - Version 1.0

This repository holds all the docker-compose.yml files for live streaming the birds of the Bird Gardens of Naples.

## Quick commands:

Startup BGON server docker containers: `sudo docker compose -f docker-compose-bgon.yml up -d`

Stop BGON server docker containers: `sudo docker compose -f docker-compose-bgon.yml down`

List all running containers: `sudo docker compose -f docker-compose-bgon.yml ps`

Update all container images: `sudo docker compose -f docker-compose-bgon.yml pull`

Delete all dangling images: `sudo docker image prune`

Check public ip address from within a container:
`sudo docker exec <container> wget http://ipecho.net/plain -O - -q ; echo`
`sudo docker exec gluetun wget http://ipecho.net/plain -O - -q ; echo`

# TODO:
* Wake on lan
* Guacamole for remote desktop