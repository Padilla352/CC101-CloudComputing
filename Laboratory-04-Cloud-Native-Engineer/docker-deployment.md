# Docker Deployment

## Checkpoint 3: Docker Environment Verification

### Docker Version

```bash
docker --version
```

This command displays the installed Docker version.

### Docker Information

```bash
docker info
```

This command displays detailed information about the Docker client and Docker server environment.

### Docker Service Status

```bash
sudo systemctl status docker
```

This command checks whether the Docker service is running. In my KillerCoda environment, the Docker service was active and running.

## Checkpoint 4: Nginx Deployment

### Pull the Nginx Image

```bash
docker pull nginx
```

This command downloads the Nginx image from Docker Hub.

### Run the Nginx Container

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

This command creates and runs an Nginx container in detached mode and maps host port 8080 to port 80 inside the container.

### List Running Containers

```bash
docker ps
```

This command displays the currently running Docker containers.

### Test the Nginx Web Server

```bash
curl http://localhost:8080
```

This command sends an HTTP request to the Nginx server through port 8080 and displays the returned HTML response.

## Checkpoint 5: Container Lifecycle

### List Running Containers

```bash
docker ps
```

This command displays the containers that are currently running.

### Stop the Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container.

### Verify the Container is Stopped

```bash
docker ps -a
```

This command displays all containers, including stopped containers, so the stopped Nginx container can be verified.

### Remove the Container

```bash
docker rm nginx-server
```

This command removes the stopped Nginx container from the Docker environment.

### Final Verification

```bash
docker ps -a
```

This command verifies that the Nginx container has been removed.
