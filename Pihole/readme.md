# Pi-hole Docker Setup

This repository provides a **Docker Compose configuration** for deploying **Pi-hole**, a powerful **network-wide ad blocker** designed to filter unwanted ads and trackers at the DNS level.  
The setup ensures **persistent storage**, customizable configurations, and optional DHCP support.

## Features
- **Comprehensive network-wide ad blocking** at the DNS level
- **Customizable DNS settings** managed via an intuitive web interface
- **Optional DHCP server mode** for managing network assignments
- **HTTPS access** secured with a self-signed certificate
- **Persistent storage** to retain configurations and logs

## Container Details
- **Utilizes the official Pi-hole image** (`pihole/pihole:latest`)
- **Exposes essential ports** for seamless network functionality:
  - `53`: DNS resolution (TCP/UDP)
  - `80`: Web-based administration interface
  - `443`: Secure HTTPS access *(self-signed certificate)*
  - *(Optional)* `67`: DHCP server functionality
  - *(Optional)* `123`: Network Time Protocol (NTP) support
- **Configuration files stored in `/Pi-Hole-Data/`** for persistence
- **Supports custom `dnsmasq` settings** for advanced configurations

## Deployment Guide

### 1. Prepare the Environment
- Place the `docker-compose.yml` file in a directory on your Docker host
- *(Optional)* Modify environment variables for timezone, password, and DNS settings

### 2. Deploy the Container
Execute the following command:
```sh
docker-compose up -d