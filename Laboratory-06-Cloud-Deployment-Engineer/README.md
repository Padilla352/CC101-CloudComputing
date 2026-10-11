# Mission 6: The Cloud Deployment Engineer

## Mission Overview

This laboratory activity demonstrates how to deploy a private cloud storage application using Docker Compose. The deployment uses Nextcloud as the web application and MariaDB as the database service. Both services are configured in a single YAML file.

## Objectives

- Understand two-tier application architecture.
- Create a Docker Compose configuration file.
- Deploy Nextcloud and MariaDB as separate containers.
- Access the Nextcloud web interface through port 8080.
- Document the deployment process using Markdown.
- Practice Infrastructure as Code (IaC).

## Commands Executed

The following commands were used to create the project directory, configure the Docker Compose file, deploy the services, check the containers, and stop the deployment.

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Database Configuration

- **Database service:** `database`
- **Database name:** `nextcloud_db`
- **Database username:** `calderon_jessy`
- **Web application:** Nextcloud
- **Database server:** MariaDB
- **Port mapping:** `8080:80`

## Skills Learned

- Docker Compose configuration
- Multi-container deployment
- YAML syntax and indentation
- Database and web application communication
- Linux command-line operations
- Technical documentation using Markdown
- GitHub portfolio management
- Infrastructure as Code (IaC)

## Screenshots

The following screenshots document the deployment, web interface, and teardown process.

### 1. Docker Compose Deployment

This screenshot shows the Nextcloud and MariaDB containers after running the Docker Compose deployment commands.

![Docker Compose Deployment](screenshots/compose-deployment.png)

**Filename:** `screenshots/compose-deployment.png`

### 2. Nextcloud Web Interface

This screenshot shows the Nextcloud installation page accessed through port 8080 in the KillerCoda environment.

![Nextcloud Web Interface](screenshots/nextcloud-web.png)

**Filename:** `screenshots/nextcloud-web.png`

### 3. Docker Compose Teardown

This screenshot shows the terminal output after the Docker Compose services have been stopped and removed.

![Docker Compose Teardown](screenshots/compose-teardown.png)

**Filename:** `screenshots/compose-teardown.png`

