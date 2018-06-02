# SWARM Linode

## commands on server

`docker swarm init --advertise-addr 139.162.249.218`

`docker info`

`docker swarm join-token manager`

`docker swarm join --token sfasdfasdfasdfasdfasf 111.111.222.218:2377`

`docker node ls`

`docker stack deploy -c docker-compose.yml getstartedlab`

`docker swarm leave --force`

## remote commands

### start app

`ssh fobos.j123.ru 'docker node ls'`

`ssh fobos.j123.ru 'docker swarm init --advertise-addr 139.162.249.218'`

`ssh deimos.j123.ru 'docker swarm join --token SWMTKN-1-4a77fwqy9szko9hf7ijhng1izy8dmdyex5ge20i1hfkm6qs6ll-62ss2lf0sljqkn533jio3nepi 139.162.249.218:2377'`

`ssh fobos.j123.ru 'docker stack deploy -c /home/mike/docker/4_swarm/docker-compose.yml getstartedlab'`

`ssh fobos.j123.ru 'docker service ls'`

`ssh fobos.j123.ru 'docker service ps getstartedlab_web'`

`ssh fobos.j123.ru 'docker stack ps getstartedlab'`

`ssh deimos.j123.ru 'docker swarm leave --force'`

`ssh fobos.j123.ru 'docker swarm leave --force'`

### scaling app

* change docker-compose.yml (commit, push, pull)
  * ssh fobos.j123.ru 'cd /home/mike/docker && git pull'
* `ssh fobos.j123.ru 'cd /home/mike/docker/4_swarm && docker stack deploy -c docker-compose.yml getstartedlab'`

### clean up

* `ssh fobos.j123.ru 'docker stack rm getstartedlab'`
