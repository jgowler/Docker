# Portainer Docker Setup

This repository provides a **Docker Compose configuration** for deploying **Portainer**, a lightweight **container management tool** featuring a web-based interface for managing Docker environments.

## Features
- **Intuitive web interface** for overseeing containers, images, networks, and volumes
- **Secure access** via HTTPS (`9443` port) for remote management
- **Seamless integration** with Docker using the `/var/run/docker.sock` socket
- **Persistent storage** ensuring configurations and settings are retained across restarts
- **Optional Edge Compute support** for managing remote environments

## Container Details
- **Uses the official Portainer image** (`portainer/portainer-ce:lts`)
- **Exposes essential ports** for accessibility:
  - `9443`: Secure HTTPS access for the Portainer web interface
  - *(Optional)* `8000`: Required for Edge Compute features
- **Ensures persistent storage**:
  - Configuration stored in the **`Portainer-data` volume**
- **Directly connects to the Docker daemon** via `/var/run/docker.sock`
- **Automatic restart** enabled unless manually stopped

## Deployment Guide

### 1. Prepare the Environment
- Place the `docker-compose.yml` file in a directory on your Docker host.

### 2. Deploy the Container
Execute the following command:
```sh
docker-compose up -d