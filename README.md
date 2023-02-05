# WPDC - WordPress Docker Compose

Easy WordPress development with Docker and Docker Compose.

## Requirements

Make sure you have the latest versions of **Docker** and **Docker Compose** installed on your machine.

Make sure to [add your user to the `docker` group](https://docs.docker.com/install/linux/linux-postinstall/#manage-docker-as-a-non-root-user) when using Linux.

## Configuration

Run the file setup before run docker-compose

```
sh setup.sh
```

Edit the file `.env` just creatd to change the MySQL root password and WordPress database name.

## Installation

Open a terminal and `cd` to the folder in which `docker-compose.yml` is saved and run:

```
docker-compose up
```

This creates new folders next to your `docker-compose.yml` file.

* `wp-app` – the location of your WordPress application

The containers are now built and running. You should be able to access the WordPress installation with url `http://localhost`.

For convenience you may add a new entry into your hosts file.

### phpMyAdmin

You can also visit `http://localhost:8080` to access phpMyAdmin after starting the containers.

The default username is `root`, and the password is the same as supplied in the `.env` file.
