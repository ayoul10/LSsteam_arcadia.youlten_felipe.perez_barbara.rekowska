# LSSteam - Arcadia Youlten, Felipe Perez, Barbara Rekowska

## Requirements

1. Docker (https://www.docker.com/products/docker-desktop)
2. Composer

## Instructions

1. After cloning the project, open your terminal and access the root folder using the cd /path/to/the/folder command.
2. To install all the dependencies run 'composer install' from the command line
3. Create a local .env file before starting the project, with the following content:

MYSQL_ROOT_USER=root

MYSQL_ROOT_PASSWORD=root

MYSQL_DATABASE=database

MYSQL_HOST=db

MYSQL_PORT=3306

SENDER=sender@gmail.com

PHP_PORT=8030

4. To start the local environment, execute the command docker-compose up -d in your terminal.
5. The above command will start the docker environment together with initialization of the database, which can be found in init/docker-entrypoint-initdb.sql

After cloning the project, make sure that the public folder and its sub directories, specifically the cache and the uploads have the appropriate permissions set (chmod 777 path_to_project_root/public/cache path_to_project_root/public/uploads),
so that the php program can read and write files to them.

## Website

Once running, access localhost:8030, and you will be redirected to the registration page.
