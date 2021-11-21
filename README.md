# Wordpress-installation-on-nginx-php_fpm


## Execution
- Running a syntax check
```sh
docker-compose config
```
- Executing the yaml file
```sh
docker-compose up -d
```


```sh
# tree .
.
├── docker-compose.yml
└── nginx-conf
    └── nginx.conf
```


```sh
# docker ps -a
CONTAINER ID   IMAGE                         COMMAND                  CREATED         STATUS         PORTS                                   NAMES
d36160095104   nginx:alpine                  "/docker-entrypoint.…"   8 minutes ago   Up 8 minutes   0.0.0.0:8080->80/tcp, :::8080->80/tcp   nginx
1c1f69f6c081   wordpress:php7.3-fpm-alpine   "docker-entrypoint.s…"   8 minutes ago   Up 8 minutes   9000/tcp                                wordpress-fpm
107631989b16   mysql:5.6                     "docker-entrypoint.s…"   8 minutes ago   Up 8 minutes   3306/tcp                                mysql
```
