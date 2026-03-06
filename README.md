# Automated AWS EKS Cluster Deployment using Terraform and Jenkins

## Project Overview

This project demonstrates how to automate the creation of an **AWS EKS (Elastic Kubernetes Service) cluster** using **Terraform** and integrate it with a **Jenkins CI/CD pipeline**. The goal is to provision cloud infrastructure automatically and deploy applications on Kubernetes with minimal manual effort.

## Architecture

* Terraform provisions AWS infrastructure.
* Jenkins pipeline triggers Terraform to create and manage resources.
* AWS EKS cluster is created with worker nodes.
* Applications are deployed to Kubernetes using kubectl.

## Tools & Technologies

* AWS (EKS, VPC, EC2, IAM)
* Terraform (Infrastructure as Code)
* Jenkins (CI/CD Pipeline)
* Docker
* Git
* Linux
  

## Features

* Automated AWS infrastructure provisioning using Terraform
* Jenkins CI/CD integration for infrastructure deployment
* Secure VPC setup with subnets and security groups
* Kubernetes cluster management using kubectl
* Scalable container orchestration with EKS

## Project Structure

```
.
├── terraform
│   ├── main.tf
│   ├── variables.tf
│   ├── outputs.tf
│
├── jenkins
│   └── Jenkinsfile
└── README.md
```

## Setup Steps


### 1. Initialize Terraform

```
terraform init
```

### 2. Plan Infrastructure(it will not creat infrastructure it gives a plan of resource)

```
terraform plan
```

### 3. Create Infrastructure(these is where actual resource is created)

```
terraform apply
```

### 5. Configure kubectl

```
aws eks update-kubeconfig --region <region> --name <cluster-name>
```

### 6. Deploy Application

```
kubectl apply -f deployment.yaml
```

## Learning Outcomes

* Hands-on experience with AWS EKS cluster setup
* Understanding Infrastructure as Code using Terraform
* CI/CD automation using Jenkins
* Kubernetes deployment and management

## Future Improvements

* Add monitoring using Prometheus and Grafana
* Implement security scanning with Trivy
* Automate application deployment using Helm

## Author
TEJAS A
Tejas
DevOps Engineer | AWS | Kubernetes | Terraform | Jenkins | Docker
