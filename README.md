# Docker Container Deployment on AWS EC2

## Project Overview

This project demonstrates deploying a Dockerized Nginx web server on an Ubuntu EC2 instance hosted on AWS. The deployment was performed using PuTTY over SSH, with Docker used to build and run a custom image serving a static HTML website.

## Architecture

Laptop
│
│ SSH (PuTTY)
▼
AWS EC2 (Ubuntu)
│
│ Docker
▼
Nginx Container
│
▼
Static Website

## Technologies Used

- AWS EC2
- Ubuntu Linux
- Docker
- Nginx
- Git
- GitHub
- PuTTY
## Project Structure

docker-deployment-project/
├── Dockerfile
├── index.html
├── README.md
├── screenshots/
└── docs/

## Prerequisites

- AWS Account
- EC2 Ubuntu Instance
- Docker Installed
- SSH Access

## Build Docker Image
bash
docker build -t docker-demo .

## Run Docker Container
bash
docker run -d -p 80:80 --name web-container docker-demo

## Verify Running Containers

bash
docker ps
## Access the Application

Open your browser:

http://<EC2-PUBLIC-IP>

## Docker Commands

Stop Container

bash
docker stop web-container

Start Container

bash
docker start web-container
Restart Container

bash
docker restart web-container
Remove Container

bash
docker rm web-containerRemove Image

bash
docker rmi docker-demo

## Screenshots

- EC2 Instance
- PuTTY Connection
- Running Container
- Browser Output

## Learning Outcomes
- Launching AWS EC2 Instances
- Connecting via SSH using PuTTY
- Installing Docker
- Building Docker Images
- Running Containers
- Managing Docker Containers
- Deploying Static Websites
- Using Git and GitHub
## Author

Snehal Awasare

GitHub:
https://github.com/awasaresnehal

LinkedIn:
https://linkedin.com/in/snehalawasare

Screenshoots 

<img width="1920" height="904" alt="EC2-runnigdockerdepoly" src="https://github.com/user-attachments/assets/8f7df574-cf55-46dd-b7c6-cbc59c840013" />



<img width="1920" height="1027" alt="puttydocker-depoly" src="https://github.com/user-attachments/assets/14e1a552-4b94-4ba1-a1be-0e5b8a4c45cd" />


<img width="1911" height="723" alt="deockerdepoly" src="https://github.com/user-attachments/assets/783c4c70-1c1c-4523-883d-544003ea4271" />

