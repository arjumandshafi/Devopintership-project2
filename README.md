Project: CI/CD Pipeline with GitHub Actions & Docker (Local Deployment)

Description:

This project demonstrates a full CI/CD pipeline.

GitHub Actions builds the image and pushes to Docker Hub.

tools used:

github 

docker desktop

VS code

Dockerhub

Steps to Use:

Clone the repository in VS code

git clone https://github.com/arjumandshafi/Devopintership-project2

cd YOUR_REPO: in this write main.yaml, dockerfile, docker-compose.yaml, app.js, package.jason 

then push the files to github repo:

git add .

git commit -m "added files"

git push -f https://github.com/arjumandshafi/Devopintership-project2

Run locally with Docker Compose:

docker-compose up

Set GitHub Secrets:

DOCKER_USERNAME

DOCKER_PASSWORD

GitHub Actions:

Builds Docker image

Pushes to Docker Hub

Pull image manually :

docker pull arjumand123/my-ci-cd-project

to access our application we need to create the container:

docker -p 3000:3000 arjumand123/my-ci-cd-project


Expected Output:

Browser should display:

Hello from GitHub Actions Pipeline!
