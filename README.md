# AWS ECS LMS Troubleshooting Project

## Project Overview
This project demonstrates deployment and troubleshooting of a containerized Learning Management System (LMS) frontend using AWS ECS Fargate.

The focus of this project is not only deployment but also diagnosing and fixing real-world cloud issues.

## Architecture Used
- Amazon ECR (Container Image Registry)
- Amazon ECS with Fargate
- Application Load Balancer (ALB)
- IAM Roles
- Security Groups
- CloudWatch Logs

## What I Did in This Project

### 1. Container Deployment
- Built and pushed a Docker image to Amazon ECR
- Deployed the LMS frontend on ECS Fargate
- Exposed the application using an Application Load Balancer

### 2. ECS Health Check Troubleshooting
- Intentionally misconfigured container health checks
- Observed task restarts and service failures
- Diagnosed issues using ECS service events and task states
- Fixed health checks using correct application endpoints

### 3. Resource Constraint Troubleshooting
- Reduced CPU and memory to simulate container crashes
- Identified stopped tasks due to resource exhaustion
- Fixed issues by allocating appropriate CPU and memory

### 4. ALB Health Check Issues
- Misconfigured ALB health check port
- Observed targets becoming unhealthy
- Fixed health check configuration to restore traffic flow

### 5. Security Group Troubleshooting
- Intentionally blocked traffic between ALB and ECS tasks
- Diagnosed connectivity issues using target group health status
- Fixed inbound security group rules to restore access

## Key Skills Demonstrated
- AWS ECS & Fargate
- Docker & Amazon ECR
- Application Load Balancer
- Cloud troubleshooting & root cause analysis
- Security Group configuration
- Real-world outage simulation and recovery

## Outcome
- Restored application availability after multiple failure scenarios
- Gained hands-on experience with production-like AWS issues

http://edutech-lms-alb-612748383.ap-south-1.elb.amazonaws.com/

## Note
This repository documents the troubleshooting process and learning outcomes.  
AWS resources are not publicly accessible, so screenshots are used as proof of work.
