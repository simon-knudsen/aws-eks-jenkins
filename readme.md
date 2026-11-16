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

<br>

# CD - Deploy to LKE cluster from Jenkins Pipeline

## Technologies used

Kubernetes, Jenkins, Linode LKE, Docker, Linux

## Project Description

This project extends the Jenkins CI/CD pipeline so that the application is deployed to a Kubernetes cluster on Linode LKE.

- Created a K8s cluster on LKE
- Installed kubectl as a Jenkins plugin
- Adjusted the Jenkinsfile to use the plugin and deploy to the LKE cluster

## Screenshots

![kubectl get node output](images/linode.png)
_The LKE cluster node is up and in Ready state._

<br>

![Jenkins pipeline stage view](images/deploy-to-lke.png)
_All pipeline stages completed successfully, including the deploy to LKE._

<br>

![kubectl get pod output](images/lke-pod-result.png)
_The nginx deployment pod is running on the LKE cluster._
