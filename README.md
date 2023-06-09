[![CircleCI](https://circleci.com/gh/Ramadhan0/microservice-kubernetes-with-aws.svg?style=svg)](https://circleci.com/gh/Ramadhan0/microservice-kubernetes-with-aws)

# Operationalize-a-Machine-Learning-Microservice-API

Microservice Project [Udacity Cloud DevOps Engineer Nanodegree]

## Project Overview

Deploy a containerized Python flask application to serve out predictions (inference) about housing prices through API calls. It uses a a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features.

### Project Procedure

- Test project code using linting
- Complete a Dockerfile to containerize this application
- Deploy containerized application using Docker and make a prediction
- Configure Kubernetes and create a Kubernetes cluster
- Deploy a container using Kubernetes and make a prediction
- Upload a complete Github repo with CircleCI to indicate the code has been tested

---

## Getting Started

### Setup the Environment

- Create a virtualenv and activate it

```
python3 -m venv <your_venv>
source <your_venv>/bin/activate
```

- Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone: `python app.py`
2. Run in Docker: `./run_docker.sh`
3. Run in Kubernetes: `./run_kubernetes.sh`

### Kubernetes Steps

- Setup and Configure Docker locally

  1. create docker account
  2. install docker locally (https://www.docker.com/get-started)

- Setup and Configure Kubernetes locally

  1. install Minikube. Follow instruction (https://minikube.sigs.k8s.io/docs/start/)
  2. install Kubernetes using Minikube (https://minikube.sigs.k8s.io/docs/start/)
  3. configure Kubernetes by running `minikube start`

- Create Flask app in Container

  1. run the shell script to build and the project in a container. `run_docker.sh`

- Run via kubectl
  1. run the shell script. `run_kubernetes.sh`
