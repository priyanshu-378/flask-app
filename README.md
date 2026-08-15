# Flask App – Docker & AWS ECS Learning Project

A simple Flask web application used as a hands-on project to learn Docker containerization and deploying containerized applications on AWS ECS.

## About

This project is part of my DevOps learning journey.

The Flask application source code is based on the **TrainWithShubham** tutorial. My primary focus in this project was learning Docker and AWS container deployment rather than developing the Flask application from scratch.

## My Contributions

### Docker

- Created a Dockerfile
- Created a multi-stage Dockerfile (`Dockerfile-multi`)
- Built Docker images locally
- Ran and tested the Flask application inside Docker containers
- Learned Docker image optimization using multi-stage builds
- Tagged Docker images for Amazon ECR

### AWS

- Created an Amazon ECR repository
- Pushed the Docker image to Amazon ECR
- Created an Amazon ECS cluster
- Created an ECS task definition
- Configured an ECS Fargate task
- Created and configured an ECS task execution IAM role
- Configured container port mapping
- Configured Security Groups for HTTP traffic
- Enabled public networking for the Fargate task
- Configured CloudWatch Logs
- Deployed and tested the Flask application on AWS ECS Fargate

## Tech Stack

- Python 3
- Flask
- Docker
- Amazon ECR
- Amazon ECS
- AWS Fargate
- Amazon CloudWatch
- AWS IAM

## Project Structure

```text
.
├── app.py
├── run.py
├── Dockerfile
├── Dockerfile-multi
├── requirements.txt
└── templates/
    └── index.html
