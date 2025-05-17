# 🖥️ Code-Server Docker Setup  

A **Docker Compose configuration** for deploying **Code-Server**, a web-based version of **VS Code**, enabling remote development in a browser.  
This setup provides a **persistent workspace**, customizable environment settings, and access control.

## 🚀 Features  
- **Self-hosted VS Code** in a browser  
- **Secure remote access** with optional password authentication  
- **Persistent workspace storage**  
- **Custom environment settings** for user preferences  
- **Easily accessible via a configured proxy domain**  

## 🔧 Container Details  
- **Runs the official Code-Server image** (`lscr.io/linuxserver/code-server:latest`)  
- **Exposes port `8443`** for accessing the web-based VS Code interface  
- **Stores configuration and workspace data** in a persistent volume (`code-server-data`)  
- **Supports password authentication** for additional security  
- **Allows customization of time zone and workspace location**  

## ⚙️ Deployment Guide  

1️⃣ **Prepare the Environment**  
- Place the `docker-compose.yml` file in a directory on your Docker host  

2️⃣ **Modify Environment Variables** (optional)  
- `PASSWORD`: Set a login password