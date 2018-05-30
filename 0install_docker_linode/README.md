# Install Docker Linode

`sudo apt-get update`

### проверка версии debian

`cat /etc/issue`

```
sudo apt-get install \
     apt-transport-https \
     ca-certificates \
     curl \
     python-software-properties
```

```
 2004  cat /etc/issue
 2005  sudo apt-get install      apt-transport-https      ca-certificates      curl      python-software-properties
 2006  curl -fsSL https://download.docker.com/linux/debian/gpg | sudo apt-key add -
 2007  sudo apt-key fingerprint 0EBFCD88
 2008  sudo add-apt-repository    "deb [arch=amd64] https://download.docker.com/linux/debian \
   $(lsb_release -cs) \
   stable"
 2009  sudo vim /etc/apt/sources.list
 2010  sudo apt-get update
 2011  sudo apt-get install docker-ce
 2012  sudo docker run hello-world
```

### далее читаем

https://docs.docker.com/install/linux/docker-ce/debian/#install-docker-ce-1
