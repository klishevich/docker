# Install Docker Linode

`sudo apt-get update`

### проверка версии debian

`cat /etc/issue`

`sudo apt-get install apt-transport-https ca-certificates curl software-properties-common`

`curl -fsSL https://download.docker.com/linux/debian/gpg | sudo apt-key add -`

`sudo apt-key fingerprint 0EBFCD88`

`sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/debian $(lsb_release -cs) stable"`

`sudo apt-get update`

`sudo apt-get install docker-ce`

`sudo docker run hello-world`

### run without sudo (security concerns)

* `sudo groupadd docker`
* `sudo usermod -aG docker $USER`
* `exit`
