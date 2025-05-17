# 🧰 Jenkins Docker Setup

A **simple Docker Compose configuration** to deploy **Jenkins**, the popular open-source **automation server**. This setup includes the **Jenkins setup wizard**, enabling quick first-time configuration.

## 🚀 What is Jenkins & Why Use It?  
Jenkins is a powerful automation tool widely used for **continuous integration (CI) and continuous delivery (CD)**. It streamlines software development by automating tasks such as **building, testing, and deployment**.  

### 🛠 Benefits of Jenkins:
- **Automates repetitive tasks** like compiling code and running tests.
- **Extends functionality** with hundreds of plugins.
- **Orchestrates complex workflows** for seamless pipeline automation.
- **Supports distributed builds** across multiple machines (agents).
- **Improves efficiency & reliability** in software development.

## 🔧 Container Details
This setup runs the **official Jenkins Docker image** with:
- **Root privileges** for full environment access.
- **Persistent storage** for Jenkins data, jobs, and configurations.
- **Exposed ports** for seamless access:
  - `8080`: Web UI for managing Jenkins.
  - `50000`: Port for Jenkins agent connections.

The **setup wizard** runs automatically on first launch, guiding you through **initial user creation, plugin installation, and basic configuration**.

## ⚙️ Usage  
To deploy Jenkins using Docker Compose:  
```sh
docker-compose up -d