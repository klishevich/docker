# Install Docker Linode

`sudo apt-get update`

### проверка версии debian

`cat /etc/issue`

`sudo apt-get install apt-transport-https ca-certificates curl software-properties-common`

`curl -fsSL https://download.docker.com/linux/debian/gpg | sudo apt-key add -`

`sudo apt-key fingerprint 0EBFCD88`

`sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/debian $(lsb_release -cs) stable"`

**Ubuntu 16.04**: `sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/debian jessie stable"`

`sudo apt-get update`

`sudo apt-get install docker-ce`

`sudo docker run hello-world`

### run without sudo (security concerns)

* `sudo groupadd docker`
* `sudo usermod -aG docker $USER`
* `exit`

## Install Mongo DB

https://www.digitalocean.com/community/tutorials/how-to-install-mongodb-on-ubuntu-16-04

## Connect to service running on host

`docker run --network host -p 8080:8080 -d 0c76faf31acc`
