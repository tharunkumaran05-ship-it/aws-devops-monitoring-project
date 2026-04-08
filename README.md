# aws-devops-monitoring-project
# End-to-End AWS DevOps Monitoring Project

## Project Overview

This project demonstrates a complete DevOps pipeline built on AWS with secure VPN access, file upload routing, CI/CD automation, monitoring, and alerting.

The architecture consists of three EC2 servers working together to simulate a production-grade DevOps environment.

---

## Architecture

Server 1
OpenVPN + Firewall
Login / Signup Website
MySQL Database

Server 2
Upload Application Server

Server 3
Jenkins CI/CD Server
Prometheus
Grafana
CloudWatch
SNS
SQS

---

## Workflow

User → VPN → Login Website → Upload File → Jenkins Pipeline → S3 / GitHub → Monitoring → Alerts

---

## File Routing Logic

Files uploaded from the application are routed automatically:

Documents and images → Amazon S3
Code files → GitHub repository

---

## AWS Services Used

EC2
VPC
Security Groups
S3
CloudWatch
SNS
SQS
IAM

---

## Tools Used

Jenkins
GitHub
Prometheus
Node Exporter
Grafana
Apache
PHP
MySQL
OpenVPN

---

## Screenshots

### EC2 Instances

![EC2](screenshots/01-ec2.png)

### VPN Disconnected

![VPN Off](screenshots/02-vpn-off.png)

### VPN Connected

![VPN On](screenshots/03-vpn-on.png)

### Homepage

![Home](screenshots/04-home.png)

### Login Page

![Login](screenshots/05-login.png)

### Signup Page

![Signup](screenshots/06-signup.png)

### Upload Page

![Upload](screenshots/07-upload.png)

### Upload Success

![Success](screenshots/08-success.png)

### S3 Bucket

![S3](screenshots/09-s3.png)

### GitHub Upload

![GitHub](screenshots/10-github.png)

### Jenkins Pipeline

![Jenkins](screenshots/11-jenkins.png)

### Prometheus Targets

![Prometheus](screenshots/12-prometheus.png)

### Grafana Dashboard

![Grafana](screenshots/13-grafana.png)

### CloudWatch Alarms

![CloudWatch](screenshots/14-cloudwatch.png)

### CPU Email Alert

![CPU](screenshots/15-cpu.png)

### Jenkins Email Alert

![Jenkins Mail](screenshots/16-jenkins-mail.png)

### SQS Email Alert

![SQS](screenshots/17-sqs.png)

---

## End-to-End Flow

1. User connects through OpenVPN
2. User signs up or logs in
3. User uploads file
4. Jenkins pipeline triggered
5. Files routed to S3 or GitHub
6. Prometheus collects metrics
7. Grafana visualizes dashboards
8. CloudWatch monitors alarms
9. SNS sends email notifications
10. SQS monitors queue messages

---

## Result

This project demonstrates a complete DevOps pipeline including:

Secure access using VPN
CI/CD automation using Jenkins
File routing to S3 and GitHub
Infrastructure monitoring
Alerting using SNS
Queue monitoring using SQS
