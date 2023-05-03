# Introduction

Welcome to the Things Solver DevOps hiring challenge! In this challenge, you will showcase your knowledge and expertise in containers and microservices by building a simple yet resilient Hello World app, deploying it to Kubernetes as a minimal container, and exposing it via a load balancer that automatically retrieves certificates from Let's Encrypt.

## The challenge consists of four main components:

- Simple Webapp: Find an example of a hello world http app in any programming language, modify it to return the message "Hello Things Solver from @YourName," and ensure it works on port 14450.

- Build the Webapp container: Create a Dockerfile that wraps the app and ensures the resulting container is as small and secure as possible. Automate the build and upload of the container using free CI services and push it to a publicly usable container registry like Docker Hub.

- TLS Offloading and Load Balancer: Research and find a suitable solution for a Kubernetes LoadBalancer infrastructure that automatically retrieves and updates Let's Encrypt certificates for any deployed service. Ensure the solution can be easily spun up within your cluster, all certificates are updated automatically, and adding a new TLS service behind the LoadBalancer is just a few lines of Kubernetes states to be applied. The app must be externally exposed on port 443 (https).

- Infrastructure Code and Scripts: Create the necessary Kubernetes configuration to deploy and tear down everything. Put them in a git repository and ensure everything is automated as much as possible, and the infrastructure is resilient.

## We suggest you follow the steps below:

- Research the technologies you plan to use.

- Create a simple hello world service, automate the build and upload of the container.

- Set up a Kubernetes cluster, use minikube, or choose a suitable option.

- Create Kubernetes YAML files, and find a way to tear everything up/down in the correct order.

- Document your setup, explaining any eventual drawbacks.

- Send back links to all git repos (using Github or Gitlab).

## We will evaluate the challenge based on the following criteria:

- Automation of all possible aspects
- Size and security of the app container
- Resilience of the infrastructure
- Documentation

__Bonus points for a diagram of the setup and if everything can be built up and deleted with one command.__