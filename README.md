[![CircleCI](https://circleci.com/gh/AO-test/project-ml-microservice-kubernetes.svg?style=svg)](https://circleci.com/gh/AO-test/project-ml-microservice-kubernetes)

## Project Overview

This project deployed a Machine Learning Microservice API.a pre-trained, sklearn model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle. This project tests your ability to operationalize a Python flask app—in a provided file, app.py—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling. This project was built using AWS Cloud 9 environment.

### Project Tasks

This project work as an operationalized machine learning microservice using Kubernetes, which is an open-source system for automating the management of containerized applications. As the following steps:
- Test your project code using linting.
- Complete a Dockerfile to containerize this application.
- Deploy your containerized application using Docker and make a prediction.
- Improve the log statements in the source code for this application.
- Configure Kubernetes and create a Kubernetes cluster.
- Deploy a container using Kubernetes and make a prediction.
- Upload a complete Github repo with CircleCI to indicate that your code has been tested.


---

## Setup the Environment

* Create a virtualenv and activate it by running this command to create python3 -m venv ~/.devops and source ~/.devops/bin/activate to activate
* Create a requirements.txt it has all packages necessary to install
* Run `make install` to install the necessary dependencies
* Run `make lint` to check that hadolint doesn't find any errors in your Dockerfile

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`
4. Run docker upload to upload docker image to your Docker hub account by using upload_docker.sh  
5. Create a directory .circleci and create a configuration file config.yml inside of it to integrate CircleCI

### To run app in a local kubernetes cluster

* Setup and Configure Docker locally by running run_docker
* Setup and Configure Kubernetes locally by running run_kubernetes
* Create Flask app in Container
* Run via kubectl   
