Remove docker if already installed <br>
$  sudo yum remove docker docker-client docker-client-latest docker-common docker-latest docker-latest-logrotate docker-logrotate docker-engine <br>
$ sudo yum update <br>
$ sudo yum install -y yum-utils <br>
$ sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo <br>
$ sudo yum install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin <br>
            DOCKER_CONFIG=${DOCKER_CONFIG:-$HOME/.docker}
