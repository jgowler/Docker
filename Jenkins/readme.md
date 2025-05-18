# Jenkins Docker Setup

This repository provides a **Docker Compose configuration** for deploying **Jenkins**, the widely used open-source **automation server**.  
The setup includes the **Jenkins setup wizard**, enabling quick first-time configuration.

## What is Jenkins & Why Use It?

Jenkins is a powerful automation tool designed for **continuous integration (CI) and continuous delivery (CD)**. It streamlines software development by automating essential tasks such as **building, testing, and deployment**.

### Benefits of Jenkins
- **Automates repetitive tasks**, including code compilation and testing
- **Extends functionality** with a vast selection of plugins
- **Orchestrates complex workflows** for seamless pipeline automation
- **Supports distributed builds** across multiple machines (agents)
- **Enhances efficiency and reliability** in software development

## Container Details
This setup utilizes the **official Jenkins Docker image**, providing:
- **Root privileges** for full environment access
- **Persistent storage** to retain Jenkins data, jobs, and configurations
- **Exposed ports** for seamless connectivity:
  - `8080`: Web UI for managing Jenkins
  - `50000`: Port for Jenkins agent connections

The **setup wizard** runs automatically on first launch, guiding users through **initial user creation, plugin installation, and basic configuration**.

## Usage
To deploy Jenkins using Docker Compose, execute:
```sh
docker-compose up -d