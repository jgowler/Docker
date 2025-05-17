# 📦 Portainer Docker Setup  

A **Docker Compose configuration** to deploy **Portainer**, a lightweight **container management tool** with a web-based interface for managing Docker environments.

## 🚀 Features  
- **Intuitive web UI** for managing containers, images, networks, and volumes  
- **Secure access** via HTTPS (`9443` port)  
- **Direct integration with Docker** using the `/var/run/docker.sock` socket  
- **Persistent storage** to retain configurations and settings across restarts  
- **Supports Edge Compute features** *(optional)*  

## 🔧 Container Details  
- **Runs the official Portainer image** (`portainer/portainer-ce:lts`)  
- **Exposes Port**:
  - `9443`: Secure HTTPS access for the Portainer web UI  
  - *(Optional)* `8000`: Needed for Edge Compute features  
- **Persistent storage**:
  - Configuration saved in the **`Portainer-data` volume**  
- **Direct Docker management**:
  - Connects to the **Docker daemon** via `/var/run/docker.sock`  
- **Auto-restart enabled** unless manually stopped  

## ⚙️ Deployment Guide  

1️⃣ **Prepare the Environment**  
- Place the `docker-compose.yml` file in a directory on your Docker host  

2️⃣ **Deploy the Container**  
Run the following command:  
```sh
docker-compose up -d
