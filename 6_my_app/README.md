# My App

## Stack

docker stack deploy -c docker-compose.yml mystack --with-registry-auth
docker service ls
docker service ps mystack_web
docker stack rm mystack

## Swarm

docker swarm init --advertise-addr 139.162.249.218
docker swarm join-token manager
docker swarm leave --force
docker node ls

## Local deploy steps

1. Stop local mongoDB
1. Login to Docker Hub `docker login`
1. create folder on local disk `/Users/mike/data` and map services.mongo.volumes in docker-compose.yml
1. Deploy stack

## if new container 

docker pull klishevich/bp-hapi-react-redux:1.0.1

## problem solving

docker service ps --no-trunc mystack_web

docker inspect -f "{{.Status.ContainerStatus.ContainerID}}" mriwtfmf7dwv

docker logs 5333edc55d3a19c3e3292e89bd931baa97fe04695a1650b100ada1942c021dc7
