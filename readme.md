# CD - Deploy to EKS cluster from Jenkins Pipeline

## Technologies used

Kubernetes, Jenkins, AWS EKS, Docker, Linux

## Project Description

This project extends an existing Jenkins CI/CD pipeline so that the application is deployed to an AWS EKS cluster.

- Installed kubectl and aws-iam-authenticator on the Jenkins server
- Created a kubeconfig file to connect to the EKS cluster and added it to the Jenkins server
- Added AWS credentials to Jenkins for AWS account authentication
- Extended the Jenkinsfile to connect to the EKS cluster and deploy to it

## Screenshots

![Jenkins pipeline stage view](images/jenkins-pipeline-k8s.png)
_All pipeline stages completed successfully, including the deploy to EKS._

<br>

![Jenkins pipeline console output](images/pipeline-logs.png)
_Pipeline logs showing the deployment created on the EKS cluster._
