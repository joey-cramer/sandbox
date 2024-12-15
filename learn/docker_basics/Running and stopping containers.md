
# The following instruction set will happen in your CLI.
# The hello-world is a simple application that outputs "Hello from Docker!" and some additional info.

# Docker CLI Commands and Flags for Running and Managing Containers

- **Run and Interact with Containers**
  - `docker run ubuntu`: Starts a container from the Ubuntu image.
  - `docker run -it ubuntu`: Runs interactively with a terminal (`-i` + `-t`).
  - `docker run -d -it --name looper ubuntu sh -c 'while true; do date; sleep 1; done'`: Starts a named, detached container running a date loop.

- **Control and Monitor Containers**
  - `docker logs -f <container>`: Follows container logs.
  - `docker pause <container>` / `docker unpause <container>`: Pauses/unpauses.
  - `docker attach <container>`: Connects to the container’s console.
  - `docker exec -it <container> <command>`: Runs commands inside a running container.

- **Stopping and Cleaning Containers**
  - `docker stop <container>`: Gracefully stops a container.
  - `docker kill <container>`: Forcefully stops the container.
  - `docker rm <container>`: Removes a stopped container.
  - `docker run --rm`: Auto-removes the container when it exits.

For more on Docker commands and flags, visit the [Docker Documentation](https://docs.docker.com/).
