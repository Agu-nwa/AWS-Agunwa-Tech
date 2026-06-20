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

