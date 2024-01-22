[日本語版 README はこちら](https://github.com/Nameless-itf23/palworld_docker/blob/master/README-ja.md)

## docker-compose for Pal World
This repository provides a docker-compose.yml file that allows you to run a Pal World dedicated server without using a Dockerfile.

## Features

- The steamapps folder inside the container is mounted to the data folder, so you can easily manage Pal World server files by directly editing them from outside the container.

### Usage

```bash
# Change directory to the cloned repository
cd path/to/this/repository

docker compose up
```

### Notes
- If the server does not start properly, it is recommended to delete the contents of the data folder.
- Set the owner and group of the data folder to a non-root user.
