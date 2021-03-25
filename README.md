# WordPress Docker

This is a docker environment designed to give you all of the tools you need to develop a wordpress site.

## Setup

1. Clone repo to project, and rename the directory.

    ```bash
    git clone https://github.com/jwoodrow99/docker-wordpress.git ~/Workspace/APP-NAME
    ```

2. Open a terminal in the cloned directory.

3. Start the docker environment.

    ``` bash
    docker-compose up -d
    ```

4. Stop the docker environment.

    ``` bash
    docker-compose down
    ```

5. Destroy the docker environment.

    ``` bash
    docker system prune -a
    ```

## Ports

* Wordpress: [localhost:8000](http://localhost:8000/)

* phpMyAdmin: [localhost:3333](http://localhost:3333/)

* MailHog: [localhost:8025](http://localhost:8025/)
