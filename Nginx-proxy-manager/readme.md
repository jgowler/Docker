# Nginx Proxy Manager Docker Setup

This repository provides a **Docker Compose configuration** for deploying **Nginx Proxy Manager (NPM)** alongside a **MariaDB database**.  
It simplifies the management of **reverse proxies, SSL certificates, and web traffic routing** via an intuitive web interface.

## Features & Components

### Nginx Proxy Manager
- **User-friendly web interface** for:
  - Reverse proxy configuration  
  - HTTP/HTTPS traffic routing  
  - Automatic **SSL certificate management** via Let's Encrypt  
- **Exposed ports**:
  - `80`: Public HTTP access  
  - `443`: Secure HTTPS traffic  
  - `81`: Admin panel  
- **Persistent storage** to retain settings and certificates:
  - Configuration stored in `./npm-data`  
  - SSL/TLS certificates saved in `letsencrypt-data`  
- **Automated container restarts** unless manually stopped  

### MariaDB Database  
- **Securely stores all Nginx Proxy Manager data**  
- **Persistent storage** maintained in the `mariadb-data` volume  
- **Automatic database upgrades** when required  
- **Ensures high availability** with automatic restarts  

## Why Use This Setup?
- Streamlines reverse proxy configuration with an intuitive interface  
- Provides automated SSL certificate management for enhanced security  
- Supports dynamic web traffic routing with minimal manual intervention  
- Ensures persistent data storage and high availability