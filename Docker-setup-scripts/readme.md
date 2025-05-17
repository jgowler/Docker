# 🐳 Docker Installation & Uninstallation Guide  

This project provides scripts to **install and uninstall Docker**, ensuring smooth setup and removal while maintaining system integrity.

## 🚀 Docker Installation  
The installation script sets up **Docker Engine, CLI, container runtime, and Docker Compose** on a Linux system.  

### 🔧 Features  
- **Secure installation** with official GPG key verification  
- **Adds Docker repository sources** for updates  
- **Installs core Docker components** for containerized environments  
- **Creates a test container** (`hello-world`) for verification  
- **Adds the current user to the `docker` group** for permission management  

### ✅ Why Use This Script?  
- Automates setup, reducing manual configuration  
- Ensures **Docker and dependencies** are installed correctly  
- Provides **user-friendly access control** for better management  

---

## ❌ Docker Uninstallation  
The removal script **completely purges Docker**, ensuring no residual data remains after removal.

### 🗑️ Features  
- **Removes all Docker packages**, including CLI and runtime dependencies  
- **Deletes stored images, containers, and volumes** to prevent leftover data  
- **Cleans up repository sources & security keys** to fully detach