# Commands

`docker swarm init`

`docker stack deploy -c docker-compose.yml`

`docker stack deploy -c docker-compose.yml getstartedlab`

## list services

`docker service ls`

## list tasks

`docker service ps getstartedlab_web`

`docker container ls -q`

## take the app down

`docker stack rm getstartedlab`

## take down the swarm

`docker swarm leave --force`
