# Code-Server Docker Setup

This repository provides a **Docker Compose configuration** for deploying **Code-Server**, a web-based version of **Visual Studio Code**, enabling remote development via a browser.  
The setup ensures a **persistent workspace**, customizable environment settings, and secure access control.

## Features
- **Self-hosted VS Code** in a browser for seamless remote development
- **Secure remote access** with optional password authentication
- **Persistent workspace storage** to maintain development environments
- **Customizable environment settings** tailored to user preferences
- **Proxy domain accessibility** for simplified access

## Container Details
- **Uses the official Code-Server image** (`lscr.io/linuxserver/code-server:latest`)
- **Exposes port `8443`** for accessing the web-based interface
- **Stores configuration and workspace data** in a persistent volume (`code-server-data`)
- **Supports password authentication** to enhance security
- **Allows customization of time zone and workspace location**

## Deployment Guide

### 1. Prepare the Environment
- Place the `docker-compose.yml` file in a directory on your Docker host.

### 2. Modify Environment Variables (optional)
- `PASSWORD`: Define a login password for secure access.