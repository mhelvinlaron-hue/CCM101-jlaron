# Docker Compose Guide

## What Does the `services:` Block Do?

The `services:` block defines the containers that make up the application. In this project, it contains two services: `database`, which uses MariaDB, and `app`, which uses Nextcloud.

## How Does Nextcloud Find the Database?

The `MYSQL_HOST=database` environment variable tells the Nextcloud application to connect to the database service named `database`. Docker Compose provides network communication between the services so the application can reach the database by its service name.

## Difference Between `docker run` and `docker-compose up -d`

The `docker run` command is used to create and start an individual container with the specified settings. The `docker-compose up -d` command uses a Compose YAML file to configure and start the services defined in that file in the background, making it easier to manage an application with multiple containers.
