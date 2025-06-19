---
title: "Aout - Order Management System"
date: 2024-01-10T10:00:00Z
draft: false
tags: ["python", "aws", "docker", "api", "backend"]
categories: ["projects"]
cover:
    image: "images/aout-architecture.png"
    alt: "Aout system architecture"
summary: "A scalable order management and dispatch advice system built with Python, deployed on AWS with Docker containerization"
---

# Aout - Order Management System

A comprehensive order management system that handles order processing and dispatch advice generation. The system is built with modern DevOps practices, featuring containerized deployment and automated testing.

## 🚀 Key Features

- **Order Processing**: Complete order lifecycle management
- **Dispatch Advice Generation**: Automated advice system for order fulfillment
- **RESTful API**: Well-documented API endpoints for integration
- **AWS Deployment**: Cloud-native architecture with Lambda functions
- **Containerized**: Docker-based deployment for consistency
- **Automated Testing**: Comprehensive test suite with CI/CD integration

## 🛠️ Technologies Used

### Backend & Core
- **Python** - Main programming language
- **Flask/FastAPI** - Web framework (based on routes.py structure)
- **RESTful APIs** - Service communication

### Cloud & Infrastructure
- **AWS Lambda** - Serverless compute
- **AWS EC2** - Virtual server instances (Used for intial version and then moved to Lambda)
- **Docker** - Containerization platform
- **Docker Compose** - Multi-container orchestration

### Development & Operations
- **GitHub Actions** - CI/CD pipeline
- **pytest** - Testing framework
- **Git** - Version control
- **SSH** - Secure server access

### Architecture Components
- **Order Management Module** (`orderClass.py`)
- **Dispatch Advice System** (`dispatchAdviceClass.py`)
- **Order-to-Advice Transfer Logic** (`OrderToAdviceTransfer.py`)
- **API Routes Handler** (`routes.py`)

## 📁 Project Structure

```
Aout/
├── model_python/          # Core business logic
│   ├── orderClass.py      # Order management
│   ├── dispatchAdviceClass.py  # Dispatch processing
│   └── OrderToAdviceTransfer.py # Transfer logic
├── python/                # Additional Python modules
├── tests/                 # Test suite
├── aws-ssh/              # AWS deployment keys
├── .github/workflows/    # CI/CD configuration
├── docker-compose.yaml   # Container orchestration
├── Dockerfile.lambda     # AWS Lambda deployment
├── Dockerfile.local      # Local development
└── requirements.txt      # Python dependencies
```

## 🔧 Deployment Options

The project supports multiple deployment strategies:

1. **Local Development**: Using `Dockerfile.local`
2. **AWS Lambda**: Serverless deployment with `Dockerfile.lambda`
3. **Testing Environment**: Isolated testing with `docker-compose.test.yml`

## 📊 Development Workflow

- **Automated Testing**: Run with `test.sh`
- **Local Execution**: Start with `run.sh`
- **CI/CD Pipeline**: GitHub Actions for automated deployment
- **Environment Management**: Configured via `env-vars`

## 🔗 Links

[View on GitHub](https://github.com/Seng2021Aout/Aout)

## 📈 Technical Highlights

- **Scalable Architecture**: Designed for high-volume order processing
- **Cloud-First Design**: Built for AWS ecosystem
- **Test-Driven Development**: Comprehensive test coverage
- **DevOps Integration**: Automated deployment and testing
- **Modular Design**: Separate concerns for orders and dispatch advice

---

*This project demonstrates proficiency in cloud-native development, containerization, and modern Python backend development practices.*