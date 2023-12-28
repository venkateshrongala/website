k8s Cluster with Auto Scaling & Auto Healing for a Apache2 Web App

# Following are the specifications of the lifecycle:
  1. Git workflow should be implemented. Since the company follows a monolithic architecture of development, you need to take care of version control.
  2. CodeBuild should be triggered once the commits are made in the master branch.
  3. The code should be containerized with the help of the Dockerfile. The Dockerfile should be built every time if there is a push to GitHub.
     Create a custom Docker image using a Dockerfile.
  4. As per the requirement in the production server, you need to use the Kubernetes cluster and the containerized code from Docker Hub should be deployed with 2 replicas.
  5. Create a NodePort service and configure the same for port 30008.
  6. Create a Jenkins Pipeline script to accomplish the above task.
  7. For configuration management of the infrastructure, you need to deploy the configuration on the servers to install necessary software and configurations.
  8. Using Terraform, accomplish the task of infrastructure creation in the AWS Cloud provider
     
# Architectural Advice:
  Softwares to be installed on the respective machines using configuration management.
  Worker1: Jenkins, Java
  Worker2: Docker, Kubernetes
  Worker3: Java, Docker, Kubernetes
  Worker4: Docker, Kubernetes
