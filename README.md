# operam_tunisia

Operam Tunisia

## Description

This repository contains the source code for a project built with Django as the backend and React as the frontend. It uses Docker and Docker Compose for containerization and MongoDB as the database.

## Technologies Used

- Django
- React
- Docker
- MongoDB

## Features

## Installation

### Backend Setup

#### Create a Virtual Environment and Install Dependencies
cd OperamTunisiaBackEnd

python -m venv venv

source venv/bin/activate  # For Linux/Mac

##### OR
venv\Scripts\activate  # For Windows

python -m pip install --upgrade pip

python -m pip install -r /requirements.txt

## Docker Commands

### View Running Containers
docker ps

### Build and Run Docker Containers
docker-compose up --build

### Stop Docker Containers
docker-compose down

### Push Docker Image to Docker Hub

#### Tag the Docker Image 
docker tag my_image:latest your_dockerhub_username/my_repository:latest

#### Log in to Docker Hub
docker login

#### Push the Docker Image to Docker Hub
docker push your_dockerhub_username/my_repository:latest



