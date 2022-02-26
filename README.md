# le-basic-nginx-image

Basic docker configuration tu run isolated laravel projects with mysql and composer as separate services

Run:

1. `docker-compose bulid`
2. `docker-compose up nginx`

To use composer run:

`docker-compose run --rm coposer [composer-comand]`

This command will run composer image execute command and after remove it 