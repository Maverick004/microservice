[![CircleCI](https://dl.circleci.com/status-badge/img/gh/Maverick004/microservice/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Maverick004/microservice/tree/master)


## Project Overview

This project aims to operationalize a Machine Learning Microservice API, built on Scikit-Learn. A pre-trained, `sklearn` model has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Project Tasks

* Test your project code using linting
* Complete a Dockerfile to containerize the application
* Deploy containerized application using Docker and initiate a prediction
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and initiate another prediction
* Integrate with CircleCI for continuous integration

Requirements

* Python 3.7

---

## Setup the Environment

* Create a virtualenv with Python 3.7 and activate it utilizing the "Makefile" file.

* Run `make install` to install the necessary dependencies

### Running Application `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker container locally by calling `./run_docker.sh`
* Setup and Configure Kubernetes locally by calling `./run_kubernetes.sh`
* Upload containerized application to Docker Hub using `./upload_docker.sh`
* Deploy Appication from dockerhub using kubernetes by running `./run_kubernetes.sh`
