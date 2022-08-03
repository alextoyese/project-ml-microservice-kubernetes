[![CircleCI](https://dl.circleci.com/status-badge/img/gh/alextoyese/project-ml-microservice-kubernetes/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/alextoyese/project-ml-microservice-kubernetes/tree/master)

OPERATIONALIZE a MACHINE LEARNING MICROSERVICE API

PROJECT OVERVIEW

In this project, you will apply the skills you have acquired in this course to operationalize a Machine Learning Microservice API.

The project entails using a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. This project tests your ability to operationalize a Python flask app—in a provided file, app.py—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

OBJECTIVE
 
The project goal is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. 


PROJECT PROCEDURE

Test project code using linting
Complete a Dockerfile to containerize this application
Deploy containerized application using Docker and make a prediction
Configure Kubernetes and create a Kubernetes cluster
Deploy a container using Kubernetes and make a prediction
Upload a complete Github repo with CircleCI to indicate the code has been tested

LIBRARIES
Docker
Hadolint
Minikube
Kubernetes


METHODOLOGY

Setup the Environment

Created a virtualenv with Python 3.7 and activate it. Refer to this link for help on specifying the Python version in the virtualenv. 

  1. python3 -m venv <your_venv>
  2. source <your_venv>/bin/activate
  
Ran make install to install the necessary dependencies

Running `app.py`

  1. Standalone:  `python app.py`
  2. Ran in Docker:  `./run_docker.sh`
  3. Ran in Kubernetes:  `./run_kubernetes.sh`

Kubernetes Steps

  1. Setup and Configured Docker locally: sign up and download docker locally
  2. Setup and Configured Kubernetes locally: Download and Installed the kubernetes using the command curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl". The next command install the kubectl, sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl.
  3. Start minikube
  3. Created Flask app in Container: Build your image using --image=$dockerpath --port=80 --labels app=name. then run the container
  4. Ran via kubectl: to get the pods and forward the container to the 
  5. run the kubernetes
