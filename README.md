# Flask App – Docker Learning Project

A simple Flask web application used to learn Docker containerization and image creation.

## About

This project is part of my DevOps learning journey.

The Flask application source code is based on the **TrainWithShubham** tutorial. My primary focus in this project was learning Docker concepts rather than developing the Flask application from scratch.

## My Contributions

* Created a Dockerfile
* Created a multi-stage Dockerfile (`Dockerfile-multi`)
* Built Docker images locally
* Tested the application inside Docker containers
* Learned Docker image optimization using multi-stage builds

## Tech Stack

* Python 3
* Flask
* Docker

## Project Structure

```
.
├── app.py
├── run.py
├── Dockerfile
├── Dockerfile-multi
├── requirements.txt
└── templates/
    └── index.html
```

## Run the Application

Build the Docker image:

```bash
docker build -t flask-app .
```

Run the container:

```bash
docker run -d -p 80:80 flask-app
```

Open in your browser:

```
http://localhost
```

Health Check:

```
http://localhost/health
```

## Learning Objectives

* Understand Docker fundamentals
* Write Dockerfiles
* Create multi-stage Docker builds
* Build and run Docker images
* Test containerized Flask applications

## Future Improvements

* Push Docker images to Amazon ECR
* Deploy the application on AWS ECS
* Add CI/CD using Jenkins or GitHub Actions
* Automate infrastructure using Terraform

## Acknowledgement

The Flask application source code is based on the **TrainWithShubham** DevOps tutorial. This repository is maintained for educational purposes, with my contributions focused on Docker containerization and related learning.
