# docker-mastery
Learn Docker and Devops. Docker Mastery: The Complete Toolset From a Docker Captain.

Docker Mastery: The Complete Toolset From a Docker Captain  
https://www.udemy.com/docker-mastery

Course Resource
* [Docker_CheatSheet](https://github.com/smalltide/docker-mastery/blob/master/resource/cheatsheet.pdf)  
* [Slides1-5](https://github.com/smalltide/docker-mastery/blob/master/resource/Slides1-5.pdf)  
* [Slides6-10](https://github.com/smalltide/docker-mastery/blob/master/resource/Slides6-10.pdf)

Skills
1. Docker
2. DevOps
3. Docker Compose
4. Docker Swarm
5. Docker Machine
6. GitHub
7. DockerHub

install docker bash completion on Mac
```
  > https://docs.docker.com/docker-for-mac/#installing-bash-completion
  > brew install bash-completion
  > ln -s /Applications/Docker.app/Contents/Resources/etc/docker.bash-completion /usr/local/etc/bash_completion.d/docker
  ln -s /Applications/Docker.app/Contents/Resources/etc/docker-machine.bash-completion /usr/local/etc/bash_completion.d/docker-machine
  ln -s /Applications/Docker.app/Contents/Resources/etc/docker-compose.bash-completion /usr/local/etc/bash_completion.d/docker-compose
```
install docker, docker-machine, docker-compose in Linux
```
  > https://store.docker.com
  > https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/
  > curl -sSL https://get.docker.com/ | sh (install latest docker using script)
  > docker version
  > sudo usermod -aG docker <linux user> (add user in docker group)
  > curl -L https://github.com/docker/machine/releases/download/v0.12.2/docker-machine-`uname -s`-`uname -m` >/tmp/docker-machine && chmod +x /tmp/docker-machine && sudo cp /tmp/docker-machine /usr/local/bin/docker-machine (install docker machine)
  > docker-machine version
  > sudo -i
  > sudo curl -L 
  https://github.com/docker/compose/releases/download/1.16.1/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose (install docker compose)
  > chmod +x /usr/local/bin/docker-compose
  > exit
  > docker-compose version  
```
start a nginx web server container
```
  > docker container run --publish 80:80 nginx (--publish for port, -p)
  > docker container run --publish 80:80 --detach nginx (--detach for run in background, -d)
  > curl 127.0.0.1
  > docker container ls
  > docker container stop <container id>
  > docker container ls -a
  > docker container run --publish 80:80 --detach --name webhost nginx (--name for define container name)
  > docker container logs webhost (watch log in webhost container)
  > docker container top webhost (watch process in webhost container)
  > docker container --help
  > docker container rm <container id> (docker container rm 4d5 834 9bc)
  > docker container rm -f <container id> (force delete docker container
```
Container VS. VM: It's Just a Process
```
  > docker container run --name mongo -d mongo
  > docker container top mongo
  > ps aux (show all running process)
  > ps aux | grep mongo
  > docker container stop mongo
  > ps aux | grep mongo
  > docker container start mongo
  > ps aux | grep mongo
```

```
  > 
  > 
  > 
  > 
  > 
  > 
```

```
  > 
  > 
  > 
  > 
  > 
  > 
```