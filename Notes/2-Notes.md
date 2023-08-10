# Environment Setup :

## Table of Contents

1. [Create Account in AWS Cloud](#create-account-in-aws-cloud)
2. [Create Linux Machine using AWS EC2 service](#create-linux-machine-using-aws-ec2-service)
3. [Connect to Linux Machine using MobaXterm OR Putty](#connect-to-linux-machine-using-mobaxterm-or-putty)
4. [Install Docker software in Linux VM](#install-docker-software-in-linux-vm)
5. [Docker Commands](#docker-commands)
6. [Docker Hub Account](#docker-hub-account)

---

## Create Account in AWS Cloud :

To get started, create an account on AWS Cloud if you don't have one already.

## Create Linux Machine using AWS EC2 service :

1. Launch an Amazon Linux EC2 instance.
2. Choose the appropriate instance type, storage, and security groups.
3. Configure the instance and choose an existing key pair or create a new one.
4. Launch the instance.

## Connect to Linux Machine using MobaXterm OR Putty link:

Use MobaXterm or Putty to connect to your Linux VM using the instance's public IP and private key.

## Install Docker software in Linux VM :

SSH into your Linux VM and follow these commands to install Docker:

```bash
$ sudo yum update -y
$ sudo yum install docker -y
$ sudo service docker start

# Add ec2-user to the docker group
$ sudo usermod -aG docker ec2-user

# Restart the session or exit and reconnect
$ exit

```

## Docker Commands :

###See Docker info
$ docker info

### List Docker images
$ docker images

### Pull the hello-world Docker image
$ docker pull hello-world

### Run the hello-world Docker image
$ docker run hello-world

### Display running Docker containers
$ docker ps

### Display all containers (running + stopped)
$ docker ps -a

### Inspect a Docker image
$ docker inspect <image-id>

### Remove a Docker image
$ docker rmi <image-name / image-id>

### Forcefully remove a Docker image
$ docker rmi -f <image-name / image-id>

### Stop a container
$ docker stop <container-id>

### Remove a Docker container
$ docker rm <container-id>

### Remove all stopped containers, unused images, and networks
$ docker system prune -a



## <span style="color:red">Note : </span>
Create account in Docker Hub (https://hub.docker.com/)