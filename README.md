
# Docker Swarm Learning Project

This repository showcases my learning journey with Docker Swarm by deploying a simple Flask application using Docker containers and Docker Compose for orchestration.


## Structure

- **Dockerfile:** Defines the container image for the Flask application.

- **docker-compose.yml:** Configures the service for Docker Swarm, including replicas, resource limits, and networking.
- **Src/** 
    - **app.py**
    - **requirement.txt**


## Learning Process

- Built the image manually using the command:
```bash
  docker build -t <Docker-Hub-username>/simple-flask-app
```
- Pushed the image to Docker Hub using:
```bash
docker push <Docker-Hub-username>/simple-flask-app
```
Swarm Deployment: Initialized Docker Swarm and deployed the stack using:
```bash
docker swarm init
docker stack deploy -c docker-compose.yml flask-app
```
## Key Learnings

- Understood the basics of Docker Swarm for orchestrating multiple containers.
- Learned to build and push Docker images to a registry (Docker Hub).
- Gained experience with docker-compose.yml for defining services, replicas, resource limits, and overlay networks.
- Troubleshooted issues with replicas not running and resolved them by pre-building the image
