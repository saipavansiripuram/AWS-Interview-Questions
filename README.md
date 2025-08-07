# AWS Interview Q&A Guide

---

## 📑 Table of Contents

### 🟢 [1. Basic AWS Questions](#1-basic-aws-questions)
- [What is AWS?](#what-is-aws)
- [What is EC2?](#what-is-ec2)
- [What is S3?](#what-is-s3)
- [Difference between S3 and EBS](#difference-between-s3-and-ebs)
- [What is an Availability Zone and Region?](#what-is-an-availability-zone-and-region)
- [What is IAM?](#what-is-iam)
- [IAM User vs IAM Role](#iam-user-vs-iam-role)
- [What is a VPC?](#what-is-a-vpc)
- [Public vs Private Subnet](#public-vs-private-subnet)
- [What is CloudWatch?](#what-is-cloudwatch)
- [What is Route 53?](#what-is-route-53)
- [AWS Pricing Models](#aws-pricing-models)

- [What is Amazon Connect?](#what-is-amazon-connect)
- [What is AWS Lambda and how does it work?](#what-is-aws-lambda-and-how-does-it-work)
- [What is DynamoDB?](#what-is-dynamodb)
- [What is SNS?](#what-is-sns)
- [What is AWS Glue?](#what-is-aws-glue)
- [What is CloudFront?](#what-is-cloudfront)
- [What is API Gateway and how does it work with Lambda?](#what-is-api-gateway-and-how-does-it-work-with-lambda)
- [What is AWS CodeCommit?](#what-is-aws-codecommit)
- [What is AWS CodePipeline?](#what-is-aws-codepipeline)
- [What is AWS Athena?](#what-is-aws-athena)
- [What is Terraform and how does it integrate with AWS?](#what-is-terraform-and-how-does-it-integrate-with-aws)

### 🔴 [3. Advanced/Scenario-Based Questions](#3-advancedscenario-based-questions)
- [How would you secure an API using IAM and API Gateway?](#how-would-you-secure-an-api-using-iam-and-api-gateway)
- [How do you monitor a serverless application in AWS?](#how-do-you-monitor-a-serverless-application-in-aws)
- [How do you manage infrastructure using Terraform for AWS?](#how-do-you-manage-infrastructure-using-terraform-for-aws)
- [How does AWS Auto Scaling work in a production environment?](#how-does-aws-auto-scaling-work-in-a-production-environment)
- [How to debug Lambda timeouts or performance issues?](#how-to-debug-lambda-timeouts-or-performance-issues)

---

## 1. Basic AWS Questions

### What is AWS?
**Answer:**  
AWS (Amazon Web Services) is a secure cloud services platform providing compute power, storage, database services, networking, machine learning, and more. It helps businesses scale and grow without upfront physical infrastructure.

---

### What is EC2?
**Answer:**  
EC2 (Elastic Compute Cloud) is a virtual server that lets you run applications in the AWS cloud. You can select different instance types optimized for memory, storage, or compute based on your application needs.

---

### What is S3?
**Answer:**  
Amazon S3 (Simple Storage Service) is an object-based storage service used to store and retrieve any amount of data from anywhere on the web. It is highly durable (99.999999999%) and supports versioning, encryption, and lifecycle rules.

---

### Difference between S3 and EBS
**Answer:**  
- **S3**: Object storage used for storing unstructured data like images, videos, backups.
- **EBS (Elastic Block Store)**: Block-level storage used as a virtual hard disk with EC2, ideal for databases and apps requiring real-time access.

---

### What is an Availability Zone and Region?
**Answer:**  
- **Region**: A geographic area (e.g., Mumbai, N. Virginia).
- **Availability Zone (AZ)**: One or more isolated data centers within a region. AZs offer fault tolerance and high availability.

---

### What is IAM?
**Answer:**  
IAM (Identity and Access Management) lets you manage users and their access to AWS resources securely. You can create users, groups, roles, and policies to fine-tune access.

---

### IAM User vs IAM Role
**Answer:**  
- **User**: Has long-term credentials; used for human users.
- **Role**: Temporary credentials; often assumed by AWS services or cross-account access.

---

### What is a VPC?
**Answer:**  
A Virtual Private Cloud (VPC) is a logically isolated network where you can launch AWS resources. You control IP ranges, route tables, internet gateways, and subnets.

---

### Public vs Private Subnet
**Answer:**  
- **Public Subnet**: Connected to Internet Gateway, accessible from the internet.
- **Private Subnet**: No direct internet access, used for backend services like databases.

---

### What is CloudWatch?
**Answer:**  
Amazon CloudWatch is a monitoring tool for AWS resources. It collects logs, metrics, and alarms, helping you track performance and troubleshoot issues.

---

### What is Route 53?
**Answer:**  
Route 53 is a scalable DNS and domain name management service. It supports routing policies (latency, weighted, failover) and integrates with health checks.

---

### AWS Pricing Models
**Answer:**  
1. **On-Demand**: Pay for usage without commitment.  
2. **Reserved Instances**: 1 or 3-year terms, lower cost.  
3. **Spot Instances**: Bid for unused capacity, very cheap.  
4. **Savings Plans**: Flexible commitment for lower rates.

---


### What is Amazon Connect?
**Answer:**  
Amazon Connect is a cloud-based contact center solution that enables businesses to set up customer service centers with low cost and easy scalability. It integrates well with Lambda, DynamoDB, and Lex for automation and analytics.

---

### What is AWS Lambda and how does it work?
**Answer:**  
Lambda is a serverless compute service that runs your code in response to events (e.g., HTTP requests, file uploads). You don’t manage servers; AWS handles provisioning and scaling. Code executes in isolated containers with defined memory and timeouts.

---

### What is DynamoDB?
**Answer:**  
Amazon DynamoDB is a NoSQL key-value and document database. It offers single-digit millisecond latency, auto-scaling, and built-in security, backup, and restore. Ideal for real-time apps like gaming, IoT, and mobile backends.

---

### What is SNS?
**Answer:**  
Simple Notification Service is a messaging service for pub/sub. It can deliver messages to multiple subscribers over HTTP, Lambda, email, SMS, etc. Used for decoupled architecture and event notifications.

---

### What is AWS Glue?
**Answer:**  
AWS Glue is a serverless ETL (Extract, Transform, Load) service used to prepare and load data for analytics. It uses Spark under the hood and integrates with S3, Redshift, Athena, and Lake Formation.

---

### What is CloudFront?
**Answer:**  
Amazon CloudFront is a content delivery network (CDN) that caches content at edge locations globally. It improves website load time and reduces latency for users around the world.

---

### What is API Gateway and how does it work with Lambda?
**Answer:**  
API Gateway is a fully managed service that allows you to create, publish, monitor, and secure APIs. It routes HTTP requests to Lambda functions (or other services), allowing you to build RESTful or WebSocket APIs.

---

### What is AWS CodeCommit?
**Answer:**  
CodeCommit is a secure, scalable, managed Git repository service. It works like GitHub or GitLab but integrates deeply with AWS IAM, CodePipeline, and CloudWatch.

---

### What is AWS CodePipeline?
**Answer:**  
CodePipeline automates your CI/CD process by modeling the release process into stages such as source, build, test, and deploy. It supports integrations with CodeBuild, Jenkins, Lambda, and more.

---

### What is AWS Athena?
**Answer:**  
Athena is an interactive query service to analyze data stored in S3 using SQL. It’s serverless, so there’s no infrastructure to manage, and you only pay for scanned data.

---

### What is Terraform and how does it integrate with AWS?
**Answer:**  
Terraform is an open-source Infrastructure as Code tool. It lets you define AWS resources in `.tf` files and manage infrastructure using version control. AWS Provider plugin helps you manage resources like EC2, IAM, S3, etc.

---

## 3. Advanced/Scenario-Based Questions

### How would you secure an API using IAM and API Gateway?
**Answer:**  
You can use **IAM roles and policies** to control who can invoke your API. By enabling IAM authorization in API Gateway, only users with valid AWS credentials and permission can access it. Combine with **Lambda authorizers** or **Cognito** for fine-grained control.

---

### How do you monitor a serverless application in AWS?
**Answer:**  
Use **CloudWatch Logs** and **Metrics** for Lambda invocations, errors, duration, and throttling. Set **alarms** for anomalies. For end-to-end tracing, use **AWS X-Ray** to see how requests flow through your serverless architecture.

---

### How do you manage infrastructure using Terraform for AWS?
**Answer:**  
Define resources in `.tf` files, run `terraform init`, `plan`, and `apply`. Use state files to track infrastructure, and modules for reusable components. Combine with **remote backends (S3)** and **state locking (DynamoDB)** for team environments.

---

### How does AWS Auto Scaling work in a production environment?
**Answer:**  
Auto Scaling adjusts the number of EC2 instances based on CloudWatch metrics (CPU, memory, etc.). It helps maintain availability and reduces cost by adding/removing instances based on traffic.

---

### How to debug Lambda timeouts or performance issues?
**Answer:**  
- **CloudWatch Logs**: Check for error stack traces or logs.
- **CloudWatch Metrics**: Monitor invocation count, duration, error rate.
- **X-Ray**: Visualize execution flow.
- **Timeout settings**: Increase timeout or memory if the function runs out.
- **Cold Start**: Pre-warm Lambdas for latency-sensitive apps.

---
