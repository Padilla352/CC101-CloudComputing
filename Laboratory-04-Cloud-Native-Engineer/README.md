# Laboratory 04 - The Cloud-Native Engineer

## Mission Overview

This laboratory activity focuses on cloud-native engineering and containerization. The activity compares traditional Virtual Machines with containers and provides practical experience using Docker in the KillerCoda Playground. An Nginx web server was deployed inside a Docker container and accessed through a mapped network port.

## Objectives

* Differentiate between Virtual Machines and containers.
* Access a Docker-enabled Linux environment.
* Execute fundamental Docker CLI commands.
* Pull and run an Nginx container.
* Configure port mapping.
* Manage the lifecycle of a Docker container.
* Document technical procedures using Markdown.
* Maintain an organized GitHub Cloud Computing Portfolio.

## Docker Commands Executed

### Checkpoint 3

```bash
docker --version
docker info
sudo systemctl status docker
```

### Checkpoint 4

```bash
docker pull nginx
docker run -d --name nginx-server -p 8080:80 nginx
docker ps
curl http://localhost:8080
```

### Checkpoint 5

```bash
docker ps
docker stop nginx-server
docker ps
docker ps -a
docker rm nginx-server
docker ps -a
```

## Skills Learned

* Docker command-line interface
* Container deployment
* Nginx deployment
* Port mapping
* Container lifecycle management
* Linux terminal usage
* Markdown documentation
* GitHub portfolio management

## Challenges Encountered

One challenge was understanding how a container differs from a traditional Virtual Machine. Another challenge was understanding port mapping and how port 8080 on the host connects to port 80 inside the Nginx container. Using the Docker commands in the KillerCoda environment helped me understand these concepts through practical experience.

