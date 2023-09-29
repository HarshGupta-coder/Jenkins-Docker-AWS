# Jenkins-Docker-AWS
End-to-End CI/CD Pipeline with Jenkins, Docker, and AWS for Building, Testing, and Deploying Node.js Apps.

# Node.js CI/CD on AWS with Jenkins and Docker

This repository contains a complete CI/CD pipeline setup using Jenkins, Docker, and AWS for building, testing, and deploying Node.js applications.

## Features

- Automated Code Deployment
- Docker Image Building and Pushing
- AWS EC2 Deployment
- GitHub Webhooks for Automation

## Prerequisites

- AWS Account with EC2 Instances
- Jenkins Installed
- Docker Installed
- GitHub Repository for Your Node.js App

## Getting Started

1. Configure Jenkins with AWS and Docker credentials.
2. Create a Jenkins pipeline using the provided `Jenkinsfile`.
3. Set up a GitHub webhook to trigger the pipeline on code changes.

## Usage

1. Push code changes to your GitHub repository.
2. Watch the Jenkins pipeline automatically build, test, and deploy your app.
3. Access your Node.js app running on AWS EC2.

## Screenshots

- [Screenshot 1: Jenkins Pipeline]  ![image](https://github.com/HarshGupta-coder/Jenkins-Docker-AWS/assets/54001485/c69b3480-9eaf-4232-bbde-b923226aa856)

- [Screenshot 2: Docker Image Build] ![image](https://github.com/HarshGupta-coder/Jenkins-Docker-AWS/assets/54001485/fd68dabe-4300-43b3-add1-8faabb4d29b7)

- [Screenshot 3: AWS EC2 Deployment] ![image](https://github.com/HarshGupta-coder/Jenkins-Docker-AWS/assets/54001485/e736415f-258d-47b2-85a5-7bd4cbfe933f)


## Credits

[Manish Negi's Blog]([https://www.example.com/blog-post](https://journeytodevops.hashnode.dev/jenkins-declarative-pipeline-with-copying-code-from-github-and-build-code-through-docker-by-pushing-the-image-to-dockerhub-and-deploying-using-aws#heading-go-to-manage-credentials-gt-add-credentials-gt-paste-private-keys-of-jenkinskeys-gtnow-go-to-configure-node-todo-cicd-and-replace-it-with-new-credentials-and-build-now)https://journeytodevops.hashnode.dev/jenkins-declarative-pipeline-with-copying-code-from-github-and-build-code-through-docker-by-pushing-the-image-to-dockerhub-and-deploying-using-aws#heading-go-to-manage-credentials-gt-add-credentials-gt-paste-private-keys-of-jenkinskeys-gtnow-go-to-configure-node-todo-cicd-and-replace-it-with-new-credentials-and-build-now)

