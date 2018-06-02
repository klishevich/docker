# Commands

`docker swarm init`

`docker stack deploy -c docker-compose.yml getstartedlab`

## list services

`docker service ls`

## redeploy

`docker stack deploy -c docker-compose.yml getstartedlab`

## list tasks

`docker service ps getstartedlab_web`

`docker container ls -q`

## take the app down

`docker stack rm getstartedlab`

## take down the swarm

`docker swarm leave --force`


## Logs reject

`docker service ps --no-trunc <service>`

`zuwyksa3pusmqh2xpoe9zbffo`

`docker inspect -f "{{.Status.ContainerStatus.ContainerID}}" zj3wej2kpfji`

