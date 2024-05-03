Remove docker if already installed \n
$  sudo yum remove docker docker-client docker-client-latest docker-common docker-latest docker-latest-logrotate docker-logrotate docker-engine \n
$ sudo yum update \n
$ sudo yum install -y yum-utils \n
$ sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo \n
$ sudo yum install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin \n
            DOCKER_CONFIG=${DOCKER_CONFIG:-$HOME/.docker}
