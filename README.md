# Operationalize-MicroService-API

[![CircleCI](https://dl.circleci.com/status-badge/img/gh/MrazTevin/Operationalize-MicroService-API/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/MrazTevin/Operationalize-MicroService-API/tree/main)

## Project Description

In this project, you will apply the skills you have acquired in this course to operationalize a Machine Learning Microservice API. This project tests your ability to operationalize a Python flask app—in a provided file, app.py—that serves out predictions (inference) about housing prices through API calls.

### Tasks to be Performed
```
1. Test your project code using linting
2. Complete a Dockerfile to containerize this application
3. Deploy your containerized application using Docker and make a prediction
4. Improve the log statements in the source code for this application
5. Configure Kubernetes and create a Kubernetes cluster
6. Deploy a container using Kubernetes and make a prediction
7. Upload a complete Github repo with CircleCI to indicate that your code has been tested
```

### Brief Description of Project Files

> * [.circleci](.circleci): Build pipeline for our microservice API
> * [model_data](model_data) : Folder that contains the pretrained `sklearn` model and housing csv files
> * [output_txt_files](output_txt_files): Folder that contains sample output logs from running `./run_docker.sh` and `./run_kubernetes.sh`
> * [app.py](app.py) : The flask application to be used
> * [Dockerfile](Dockerfile): Has instructions to containerize the application
> * [Makefile](Makefile) : Has instructions for the environment setup and lint tests
> * [requirements.txt](requirements.txt): list of required dependencies
> * [run_docker.sh](run_docker.sh): a bash script to build Docker image and run the application in a Docker container
> * [upload_docker.sh](upload_docker.sh): a bash script to upload the built Docker image to Dockerhub
> * [run_kubernetes.sh](run_kubernetes.sh): a bash script to run the application in a Kubernetes cluster
> * [make_prediction.sh](make_prediction.sh): a bash script to make predictions against the Docker container and k8s cluster
> * [README.md](README.md): project's README file
> * [Project_Screenshots](Project_Screenshots): Checkout the screenshots that I took, while building this project 

### Instructions to get started

1. Create and activate a virtual environment.
2. Run ```make install``` and get the required dependencies.

### Run the Flask App

```
1. Standalone: python3 app.py
2. Using docker:
      ./run_docker.sh
3. With Kubernetes:
      ./run_kubernetes.sh
```
### Using Kubernetes

```
* Configure Docker locally.
* Configure Kubernetes locally.
* Containerize the flask application.
* Use kubectl to get the application running
```
    
