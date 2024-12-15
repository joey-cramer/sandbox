# Docker CLI Basics
See full instruction set at [Docker](https://docs.docker.com/ 'Docker documentation')


### Run and Manage Containers
- **Run a Container:** `docker container run <image>` — Start a container from an image.
  - Shorthand: `docker run <image>`
- **List Containers:** `docker container ls` — Shows running containers; add `-a` for all containers (including stopped).
  - Shorthand: `docker ps`
- **Stop a Container:** `docker container stop <container>` — Gracefully stop a running container.
- **Remove a Container:** `docker container rm <container>` — Remove a stopped container.

### Image Management
- **List Images:** `docker image ls` — Shows all downloaded images.
  - Shorthand: `docker images`
- **Remove an Image:** `docker image rm <image>` — Deletes a specified image.
  - Shorthand: `docker rmi`
- **Download an Image:** `docker image pull <image>` — Pulls an image from Docker Hub.
  - Shorthand: `docker pull`

### Other Useful Commands
- **Exec Command in Container:** `docker container exec <container> <command>` — Run commands inside a running container.
  - Shorthand: `docker exec`
- **Remove All Stopped Containers:** `docker container prune` — Cleans up unused containers.
- **Clean System:** `docker system prune` — Removes all stopped containers, unused networks, dangling images, and build cache.

### Basic Usage Example:
1. Run `docker container run hello-world` to start a basic test container.
2. Use `docker container ls -a` to view all containers.
3. Clean up with `docker container prune` to remove all stopped containers.



# Docker CLI Flags Reference

- **`-a` (all)** — Lists all items, not just active ones. Common with:
  - `docker container ls -a`: Lists all containers, including stopped ones.
  - `docker image ls -a`: Lists all image layers, including intermediate layers.

- **`-d` (detached)** — Runs containers in the background (detached mode). Useful in:
  - `docker run -d <image>`: Starts a container in the background.

- **`-it` (interactive + TTY)** — Runs interactively with terminal access, ideal for shell sessions.
  - `docker run -it <image>`: Launches a container interactively.
  - `docker exec -it <container> <command>`: Accesses a running container shell.

- **`--rm`** — Automatically removes a container when it stops.
  - `docker run --rm <image>`: Starts a container that deletes itself after stopping.

- **`-p` (publish)** — Maps container ports to the host.
  - `docker run -p <host_port>:<container_port> <image>`: Maps specified ports for access.

- **`--name`** — Assigns a custom name to the container for easy reference.
  - `docker run --name <name> <image>`: Starts a container with a specified name.

- **`--volume` or `-v`** — Mounts host directory as a volume in the container.
  - `docker run -v <host_path>:<container_path> <image>`: Binds a local path to a container path.

- **`--env` or `-e`** — Passes environment variables to a container.
- `docker run -e MY_VAR=value <image>`: Sets environment variables.



# Docker examples

<implement more when time>