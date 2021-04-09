# WordPress Docker

This is a docker environment designed to give you all of the tools you need to develop and manage a wordpress site.

## Prerequisites

* [Docker Desktop](https://www.docker.com/products/docker-desktop) (MacOS and Windows)

* [Docker Engine](https://docs.docker.com/engine/install/) (Linux)

* [Docker Compose](https://docs.docker.com/compose/install/) (Linux)

## Setup

1. Clone repo to project, and rename the directory (replace "WEBSITE-NAME" with the name of your website).

    ```bash
    git clone https://github.com/jwoodrow99/docker-wordpress.git ~/Workspace/WEBSITE-NAME
    ```

2. Open a terminal in the cloned directory.

3. Start the docker environment.

    ``` bash
    docker-compose up -d
    ```

4. Go to [localhost:8000](http://localhost:8000/) and follow the WordPress setup.

5. Stop the docker environment.

    ``` bash
    docker-compose down
    ```

6. Destroy the docker environment.

    ``` bash
    docker system prune -a
    ```

## Reset Project

All relivent data is stored in the ```/data``` directory, with image specific data stored in a subdirectory with the name of the related image. This allows for the docker container and images to be destroyed and built again without loosing any data, as well as backing up your project. To fully reset the container delete the ```/data``` directory and build the container again.

## Ports

* Wordpress: [localhost:8000](http://localhost:8000/)

* phpMyAdmin: [localhost:3333](http://localhost:3333/)

* MailHog: [localhost:8025](http://localhost:8025/)

## Passwords

* MySQL Root:
  * **Username**: root
  * **Password**: root

* MySQL User:
  * **Username**: wordpress
  * **Password**: password
