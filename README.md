# CI/CD Kubernetes Cluster with Jenkins

This project provides a simple Infrastructure-as-Code setup for deploying a Kubernetes-based CI/CD environment using Vagrant, Ansible, Docker, Jenkins, and Kubernetes.

The goal is to quickly provision a local multi-node Kubernetes cluster and demonstrate a basic CI/CD workflow where Jenkins builds and deploys applications into Kubernetes.

## Components

- Vagrant -> Creates and manages virtual machines
- VirtualBox -> VM provider used by Vagrant
- Ansible -> Automates cluster configuration and provisioning
- Docker -> Container runtime
- Kubernetes (K8s) -> Container orchestration platform
- Jenkins -> CI/CD automation server
- GitHub -> Source code repository integration

## Architecture

- 1 Kubernetes Master Node
- Worker Node(s)
- Jenkins server integrated into the cluster
- Automated provisioning using Ansible playbooks

## Requirements

Install the following tools before starting.

### Ubuntu/Debian

```bash

sudo apt update

```

### Install VirtualBox
```bash
sudo apt install -y virtualbox
```

### Install Vagrant
```bash

wget https://releases.hashicorp.com/vagrant/2.4.1/vagrant_2.4.1-1_amd64.deb

sudo dpkg -i vagrant_2.4.1-1_amd64.deb
```

### Verify Installation
```bash

vagrant --version

virtualbox --version
```

## Quick Start

Clone the repository:
```bash

git clone https://github.com/ahmad-bensalah/CI-CD_K8S_Jenkins.git

cd CI-CD_K8S_Jenkins
```

Start and provision the full infrastructure:
```bash

vagrant up --provision
```

The cluster, Jenkins, and required services will be automatically configured.

## Features

- Automated Kubernetes cluster deployment
- Jenkins CI/CD integration
- Infrastructure as Code using Ansible
- Reproducible local DevOps environment
- Beginner-friendly Kubernetes lab setup

## Notes

- First provisioning may take several minutes depending on internet speed and machine resources.
- Ensure virtualization is enabled in BIOS.
- Recommended RAM: 8 GB or more.

