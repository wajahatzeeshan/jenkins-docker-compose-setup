# Jenkins Tutorial Files

### Starting the containers

- to start jenkins, use `docker-compose up -d node`

- If you prefer to build images yourself, append `-f build-docker-compose.yaml` after `docker-compose`. For example, to build the `node` tutorial Jenkins instance, use: `docker-compose -f build-docker-compose.yaml up -d node`.

### How to Verify Jenkins Installation

- Check the status of the container with the `docker ps` or `docker-compose ps` commands.
- Access your running Jenkins instance at [http://127.0.0.1:8080](http://127.0.0.1:8080).

### Clean Up Instructions

- To stop and remove running containers, use `docker compose down`.
- If you encounter a `Resource is still in use` warning, use the `--remove-orphans` option which would give `docker-compose down --remove-orphans`.
- To remove the created volumes (should you need to restart from scratch), add the `-v` option which would give `docker-compose down -v`.
