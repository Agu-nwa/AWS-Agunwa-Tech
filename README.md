# 💻 Agunwa Technologies - AWS DevOps Portfolio

## 👋 Overview
This repository documents my hands-on AWS Cloud & DevOps engineering practice, focusing on real-world infrastructure design, deployment, and high availability systems.

The goal of this project is to simulate production-level cloud architecture using AWS services such as EC2, EBS, Elastic IPs, and Load Balancers.

---

# 🧠 Project Challenge (Real-World Scenario)

## 🏢 Company Requirement
Agunwa Technologies wants to deploy a highly available web application on AWS.

You have been hired as a Cloud/DevOps Engineer to design and implement the infrastructure.

---

## 🎯 Project Objectives

You are required to:

### 1. Compute Layer (EC2)
- Launch **3 Ubuntu EC2 instances**
- Install and configure **Nginx**
- Each server must return a unique response to identify itself

Example:
- Server 1 → "Welcome to Agunwa Tech - Server 1"
- Server 2 → "Welcome to Agunwa Tech - Server 2"
- Server 3 → "Welcome to Agunwa Tech - Server 3"

---

### 2. Storage Layer (EBS)
- Attach an additional **EBS volume**
- Format using **ext4 filesystem**
- Mount to a directory:

- # 🚀 Agunwa Tech - AWS DevOps Setup

## 🧭 Project Initialization (Git Setup)

This section documents the initial setup of the project repository and Git remote configuration.

---

## 📁 1. Create Project Directory

### Command
```bash
mkdir Agunwa-tech

A new project folder named Agunwa-tech was created in the home directory

# 📂 Project Setup Steps (Git Initialization Phase)

This section documents the initial setup of the Agunwa Tech DevOps project, including navigation into the project directory, Git initialization, and remote repository configuration.

---

## 📁 1. Navigate into Project Directory

### 🧾 Command
```bash
cd ~/Agunwa-tech
Successfully moved into the project workspace directory:

## 📁 1.1: Git initialization

### Command
```bash
git init
Initialized empty Git repository in /Users/gillisokolov/.git/

## 📂 1.2: Add Remote GitHub Repository
```bash
git remote add origin https://github.com/Agu-nwa/AWS-Agunwa-Tech.git

Remote repository successfully linked to local project.

This allows synchronization between local development environment and GitHub remote repository.

## 📂 1.3: Verify Remote Connection

### Command
```bash
git remote -v

origin	https://github.com/Agu-nwa/AWS-Agunwa-Tech.git (fetch)
origin	https://github.com/Agu-nwa/AWS-Agunwa-Tech.git (push)


# 🖥️ EC2 Instance Deployment

## 🚀 1. Launch EC2 Instance

### Configuration
- Instance Names: Server1 Server2 Server3
- OS: Ubuntu Linux
- Instance Type: t2.micro
- Security Group Rules:
  - SSH (22)
  - HTTP (80)

---

### Result
EC2 instance successfully launched and running in AWS cloud environment.

### Verification
- Instance state: Running
- Public IP: Assigned
- SSH access: Enabled


