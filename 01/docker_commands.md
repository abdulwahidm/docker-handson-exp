## Practice Steps

1. Build Docker Image

```
docker build -t my-bash-curl-app
``` 
Build a Docker image named "my-bash-curl-app" using the provided Dockerfile.

2. Run Docker Container

```
docker run --rm my-bash-curl-app
```
Run a Docker container from the "my-bash-curl-app" image and observe the output.

3. View Running Containers

```
docker ps
```
View the list of running containers. Ensure the container from the "my-bash-curl-app" image is no longer running.

4. Run Docker Container with Interactive Shell

```
docker run -it --rm my-bash-curl-app /bin/bash
```
Run a Docker container and enter an interactive shell inside it.

5. View Logs of a Stopped Container

```
docker ps -a
```
docker logs <container_id>
If the container has stopped, view its logs using the container ID.

6. View Created Docker Images

```
docker images
```
View a list of all Docker images created on system.

7. Remove Unused Docker Images

```
docker image prune
```
Remove unused Docker images.

8. Conclusion
This hands-on practice guides through Dockerizing a Bash and Curl application, creating a Docker image, and running containers. It demonstrates the basic usage of Docker commands and provides a foundation for containerizing more complex applications.