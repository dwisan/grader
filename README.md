> Preparing 
```
$ sudo apt update
$ sudo apt install atop
```
> Installing Docker
```
$ sudo apt install apt-transport-https ca-certificates curl software-properties-common
$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
$ sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"
$ sudo apt update
$ sudo apt install docker-ce
$ sudo systemctl status docker
$ sudo usermod -aG docker ${USER}

source: https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-18-04
```

> Installing docker-compose
```
$ sudo curl -L https://github.com/docker/compose/releases/download/1.21.2/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose
$ docker-compose --version
```
> Installing submission
```
$ cd /home
$ tar xfvz /tmp/submission.tgz
$ cd submission
$ nano docker-compose.yml
```
> Start Submission
```
$ cd /home/submission
$ docker-compose up -d
```
> Install grader
```
$ sudo apt-get install g++-multilib
$ sudo apt-get install  libmysqlclient-dev
$ sudo apt-get install  build-essential
$ sudo apt-get install  gcc g++
$ cd /home
$ tar xfvz /tmp/grader-compiled.tgz
$ cd /home/grader-compiled
$ nano grader.conf
```
> runing grader
```
$ cd /home/grader
$ ./grader toi
```
