# Cloud-native-Monitoring-app

This Application will give the CPU and Memory Utilization of the particular  system which is further deployed on EKS cluster.

Details of files:
app.py:This python file is the main backed file . I have used psutil, and flask framework to create this application which will show real time CPU and Memory Utilization of the System.
Template: this file consist of html file which will be the UI of the application.
Dockerfile: Dockerfile consist of all the step require to install and run the application in any machine. For that we need to use docker build command to create a image file then docker run to execute a image to create container.
Ecr.py: This code helps to create ECR repository witchout help of aws console. I have used boto3 module for this.
Eks.py: Consist of K8s manifest files to deploy the application in K8s cluster.

Steps to Deploy on EKS Cluster

1:Create a ECR Repo
 
2:Push Particular image into ecr repo

3:Create a EKS Cluster

4: Deploy the Application
 
