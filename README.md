# Docker LNMP Environment using MariaDB 10.3

Docker container with Nginx/Adminer/MariaDB 10.3/PHP 5.6/PHP 7.3

Thanks to https://labs.play-with-docker.com/ , we can try the environment easily. Just click below:

[![Try in PWD](https://raw.githubusercontent.com/play-with-docker/stacks/master/assets/images/button.png)](https://labs.play-with-docker.com/?stack=https://raw.githubusercontent.com/bitplus/docker-lnmp-10.3/compose/stack.yml) Then execute commands below:

```shell
docker stack rm pwd
git clone https://github.com/bitplus/docker-lnmp-10.3
cd docker-lnmp-10.3
bash start.sh
```

------

Start using docker-compose:

```bash
git clone https://github.com/bitplus/docker-lnmp-10.3
cd docker-lnmp-10.3
docker-compose up -d
```

Stop using docker-compose:

```shell
docker-compose down
```

Status:

```shell
docker-compose ps
```

------

Start using docker swarm:

`bash start.sh` or `docker stack deploy -c stack.yml lnmp`

Stop using docker swarm:

```shell
docker stack rm lnmp
```

Status:

```shell
docker stack ps lnmp --no-trunc
```

------

Notes:

If running Docker swarm, the path of directory structure must exist on every swarm node (also on manager). Otherwise, you will get error 'invalid mount config for type "bind": bind source path does not exist'.



Branch `main` is for Dockerfile updates and [Docker Hub](https://hub.docker.com/r/dtstudio/php) auto build.

Branch `compose` is for normal YAML files updated.

