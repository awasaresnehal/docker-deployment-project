# Docker Deployment on AWS EC2

## Project Overview
This project demonstrates deploying a static website inside a Docker container on an Ubuntu EC2 instance.

## Technologies Used
- AWS EC2
- Ubuntu Linux
- Docker
- Git
- GitHub
- PuTTY

## Steps
1. Launch an EC2 instance.
2. Install Docker.
3. Create a Dockerfile.
4. Build the Docker image.
5. Run the Docker container.
6. Access the website using the EC2 public IP.

## Docker Commands

```bash
docker build -t docker-demo .
docker run -d -p 80:80 --name web-container docker-demo
```
