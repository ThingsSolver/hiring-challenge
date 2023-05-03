# Introduction

Welcome to the Things Solver DevOps hiring challenge! This challenge is designed to test your skills in transferring a Lambda function to a FastAPI Docker service with Prometheus and Grafana monitoring. The goal is to create a dockerized application that exposes app metrics and displays them on a Grafana dashboard.

# Requirements

To complete this challenge, you will need to have the following software installed on your system:

- Docker
- Docker Compose
- A code editor (e.g. VS Code)

## Steps

Follow the steps below to complete the challenge:

### Step 1: Transfer Lambda Function to FastAPI Docker Service

Use handler.py function for this excercise. Once you have the code ready, create a Dockerfile to build the Docker image for your application.

### Step 2: Put the Docker Service in Docker Compose

Once you have built the Docker image, put it in a Docker Compose file. This file should define a service for your application that uses the Docker image you created in the previous step.

### Step 3: Expose App Metrics with Prometheus and Grafana

The next step is to expose app metrics with Prometheus and Grafana. Please use CAAdvisor for this step.

### Step 4: Create Grafana Dashboard with Exposed Total Memory Consumption and Network Traffic

With Prometheus and Grafana set up, the next step is to create a Grafana dashboard that displays the metrics exposed by your application. Specifically, the dashboard should display total memory consumption and network traffic.

### Step 5: Docker-Compose Up Should Bring Everything Up and Running

Finally, test your application by running docker-compose up. This should bring up all the containers and allow you to view the metrics on the Grafana dashboard.

## Evaluation criteria
- The lambda functions are pretty simple, we expect the resulting FastAPI application to be equally simple. Even if you don't know python, the FastAPI documentation should provide enough guidance
- The Dockerfile and your changes to docker-compose.yml are sensible and concise. You can talk about the pros and cons of your setup in relation to convenience vs security.
- You document your process
- It works reliably. `docker-compose up` and your documentation should be all that is required to review your solution