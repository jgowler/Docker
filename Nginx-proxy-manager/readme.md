# 🛡️ Nginx Proxy Manager Docker Setup

A **Docker Compose configuration** for deploying **Nginx Proxy Manager (NPM)** alongside a **MariaDB** database.  
This setup allows easy management of **reverse proxies, SSL certificates**, and **web traffic routing** through an intuitive web interface.

## 🚀 Features & Components

### 🔀 Nginx Proxy Manager
- **Intuitive Web UI** to manage:
  - Reverse proxy configurations  
  - HTTP/HTTPS traffic routing  
  - Automatic **SSL certificate management** via Let's Encrypt  
- **Exposed Ports**:
  - `80`: Public HTTP access  
  - `443`: Secure HTTPS traffic  
  - `81`: Admin panel  
- **Persistent storage** for proxy settings and certificates:
  - Configuration stored in `./npm-data`  
  - SSL/TLS certificates saved in `letsencrypt-data`  
- **Automated container restart** unless stopped manually  

### 🗄️ MariaDB Database  
- **Stores all Nginx Proxy Manager data** securely  
- **Persistent storage** in `mariadb-data` volume  
- **Automatic database upgrades** when required  
- **Ensures high availability** by restarting when needed  

## 🔧 Why Use This Setup