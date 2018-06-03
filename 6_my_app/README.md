# My App

ssh fobos.j123.ru 'cd /home/mike/docker && git pull'

ssh fobos.j123.ru 'cd /home/mike/docker/6_my_app && docker stack deploy -c docker-compose.yml getstartedlab'

## Stack

docker stack deploy -c docker-compose.yml mystack --with-registry-auth

docker service ls

docker service ps mystack_web

docker stack rm mystack

## Swarm

docker swarm join-token manager

docker swarm leave --force

docker swarm init --advertise-addr 139.162.249.218

docker node ls

## if new container 

docker pull klishevich/bp-hapi-react-redux:1.0.1

## problem solving

docker stack rm getstartedlab

docker stack deploy -c docker-compose.yml getstartedlab

docker service ls

docker service ps getstartedlab_web

docker service ps --no-trunc getstartedlab_web

docker inspect -f "{{.Status.ContainerStatus.ContainerID}}" mriwtfmf7dwv

docker logs 5333edc55d3a19c3e3292e89bd931baa97fe04695a1650b100ada1942c021dc7
