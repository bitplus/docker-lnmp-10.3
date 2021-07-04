# docker-lnmp-10.3

Docker container with Nginx/Adminer/MariaDB 10.3/PHP 5.6/PHP 7.3



Start using docker-compose:

```bash
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



