# My App

`ssh fobos.j123.ru 'cd /home/mike/docker && git pull'`

`ssh fobos.j123.ru 'cd /home/mike/docker/6_my_app && docker stack deploy -c docker-compose.yml getstartedlab'`

## problem solving

`docker stack rm getstartedlab`

`docker stack deploy -c docker-compose.yml getstartedlab`

`docker service ls`

`docker service ps getstartedlab_web`

`docker service ps --no-trunc getstartedlab_web`
