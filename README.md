<h1>Remove docker if already installed </h1><br>
<h2>$  sudo yum remove docker docker-client docker-client-latest docker-common docker-latest docker-latest-logrotate docker-logrotate docker-engine</h2><br>
<h2>$ sudo yum update </h2><br>
<h2>$ sudo yum install -y yum-utils </h2><br>
<h2>$ sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo</h2> <br>
<h2>$ sudo yum install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin </h2><br>
            <h2>To Install for current user:-</h2> <br>
            <h3>DOCKER_CONFIG=${DOCKER_CONFIG:-$HOME/.docker}</h3><br>
            <h3>mkdir -p $DOCKER_CONFIG/cli-plugins</h3><br>
            <h3>curl -SL https://github.com/docker/compose/releases/download/v2.27.0/docker-compose-linux-x86_64 -o $DOCKER_CONFIG/cli-plugins/docker-compose</h3><br>
            <h3>chmod +x $DOCKER_CONFIG/cli-plugins/docker-compose</h3><br>
            <h2>To Install for all users:-</h2><br>
            <h3>mkdir -p /usr/local/lib/docker/cli-plugins</h3><br>
            <h3>DOCKER_CONFIG=${DOCKER_CONFIG:-/usr/local/lib/docker}</h3><br>
            <h3>mkdir -p $DOCKER_CONFIG/cli-plugins</h3><br>
            <h3>curl -SL https://github.com/docker/compose/releases/download/v2.27.0/docker-compose-linux-x86_64 -o $DOCKER_CONFIG/cli-plugins/docker-compose</h3><br>
            <h3>chmod +x $DOCKER_CONFIG/cli-plugins/docker-compose</h3><br>
            <h3>./$DOCKER_CONFIG/cli-plugins/docker-compose --version</h3>
