# Flask App - Docker & AWS ECS Deployment

A simple Flask web application containerized with Docker and deployed on AWS ECS as part of my DevOps learning journey.

## About

This project was created for learning Docker and AWS ECS deployment.

The Flask application source code is based on the **TrainWithShubham** tutorial. My focus was on understanding the containerization and deployment process rather than developing the application itself.

## My Contributions

- Created a Dockerfile
- Created a multi-stage Dockerfile
- Built Docker images
- Ran and tested containers locally
- Tagged and pushed Docker images
- Deployed the application on AWS ECS
- Verified application health using the `/health` endpoint

## Tech Stack

- Flask
- Python
- Docker
- AWS ECS
- Amazon ECR

## Project Structure

```
.
├── app.py
├── run.py
├── requirements.txt
├── Dockerfile
├── Dockerfile-multi
└── templates/
    └── index.html
```

## Run Locally

```bash
docker build -t flask-app .
docker run -p 80:80 flask-app
```

Open:

```
http://localhost
```

Health Check:

```
http://localhost/health
```

## Learning Objectives

- Writing Dockerfiles
- Multi-stage Docker builds
- Docker image optimization
- Running containers
- Amazon ECR
- AWS ECS deployment

## Acknowledgement

The Flask application source code is based on the **TrainWithShubham** DevOps tutorial. This repository is maintained for educational purposes, with my primary contributions focused on Docker containerization and AWS ECS deployment.
