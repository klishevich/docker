# Stacks

opened ports `netstat -ntpl`

## Deploy

`ssh fobos.j123.ru 'cd /home/mike/docker/5_stacks && git pull && docker stack deploy -c docker-compose.yml getstartedlab'`

`ssh fobos.j123.ru 'docker service ls'`
`ssh fobos.j123.ru 'docker stack rm getstartedlab'`
`ssh fobos.j123.ru 'cd /home/mike/docker/5_stacks && docker stack deploy -c docker-compose.yml getstartedlab'`
