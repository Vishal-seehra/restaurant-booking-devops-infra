# 🍽️ Restaurant Booking Management System (DevOps Project)

![AWS](https://img.shields.io/badge/AWS-Cloud-orange)
![Docker](https://img.shields.io/badge/Docker-Containerization-blue)
![Prometheus](https://img.shields.io/badge/Prometheus-Monitoring-yellow)
![Grafana](https://img.shields.io/badge/Grafana-Dashboard-orange)
![Terraform](https://img.shields.io/badge/Terraform-IaC-purple)
![CI/CD](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

## 🚀 Project Overview

This project is a **full-stack restaurant booking system** deployed using a complete **DevOps pipeline** on AWS.
It demonstrates **end-to-end system design**, including infrastructure provisioning, monitoring, logging, security, and CI/CD automation.

---

## 🏗️ Architecture

```
User → ALB → EC2 (Docker Containers)
                  ├── Frontend (Nginx)
                  ├── Backend (Java API)
                  ├── Prometheus
                  └── Grafana

Backend → RDS (MySQL)

Logs → CloudWatch
Alerts → SNS
Security → IAM + WAF
IaC → Terraform
CI/CD → GitHub Actions
```

---

## ⚙️ Tech Stack

### 💻 Frontend

* HTML5
* CSS3
* JavaScript

### 🔧 Backend

* Java (HTTP Server)
* REST API

### 🗄️ Database

* MySQL (AWS RDS)

### ☁️ Cloud & DevOps

* AWS EC2 (Compute)
* AWS ALB (Load Balancer)
* AWS RDS (Database)
* Docker & Docker Compose
* Prometheus & Grafana
* CloudWatch Logs & Insights
* SNS (Alerts)
* AWS Budgets
* Terraform (Infrastructure as Code)
* GitHub Actions (CI/CD)

---

## 🚀 Features

* 📅 Table Reservation System
* 👥 Customer Management
* ⚡ Real-time Backend API
* 🐳 Containerized Deployment
* 📊 Monitoring with Prometheus & Grafana
* 📜 Centralized Logging with CloudWatch
* 🔔 Alerting via SNS
* 💰 Cost Monitoring with AWS Budgets
* 🔐 Security with IAM & WAF
* ⚙️ Fully Automated CI/CD Pipeline
* 🏗️ Infrastructure as Code using Terraform

---

## 🔄 CI/CD Pipeline

* Trigger: Push to `main` branch
* Steps:

  1. Pull latest code on EC2
  2. Stop running containers
  3. Rebuild Docker images
  4. Restart services

---

## 📊 Monitoring & Logging

### 📈 Metrics

* Prometheus scrapes backend metrics
* Grafana dashboards visualize:

  * Request count
  * System performance

### 📜 Logs

* Logs → CloudWatch
* Query logs using CloudWatch Insights

### 🔔 Alerts

* Error-based alerts using CloudWatch + SNS
* Email notifications for failures

---

## 🔐 Security

* IAM roles for secure access
* WAF rules to protect ALB
* Security Groups for controlled traffic

---

## 💰 Cost Optimization

* AWS Budgets configured
* Alerts at 75% and 100% usage

---

## 🏗️ Infrastructure as Code

Terraform is used to:

* Provision EC2 instances
* Configure security groups
* Automate infrastructure setup

---

## 📦 Deployment

### 🔹 Manual (Initial Setup)

```bash
docker-compose up --build -d
```

### 🔹 Automated (CI/CD)

* Push code → Auto deploy via GitHub Actions

---

## 🌐 Live Application

```
http://restaurant-alb-1171895923.eu-north-1.elb.amazonaws.com/
```

---

## 🧠 Learnings

* End-to-end DevOps pipeline implementation
* Real-world AWS architecture design
* Monitoring, logging, and alerting systems
* CI/CD automation using GitHub Actions
* Infrastructure automation using Terraform

---

## 🏆 Key Highlights

✔ Production-grade architecture
✔ Fully automated deployment
✔ Scalable and secure design
✔ Real-time monitoring & alerts
✔ Cost-aware cloud usage

---

## 👨‍💻 Author

**Vishal Seehra**
