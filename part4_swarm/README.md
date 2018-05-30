# SWARM Linode

`sudo docker swarm init --advertise-addr 139.162.249.218`

`sudo docker info`

`sudo docker swarm join-token manager`

`sudo docker swarm join --token sfasdfasdfasdfasdfasf 111.111.222.218:2377`

`sudo docker node ls`

`sudo docker stack deploy -c docker-compose.yml getstartedlab`

`sudo docker swarm leave --force`
