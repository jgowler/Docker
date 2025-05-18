# Cloudflare Dynamic DNS (DDNS) Docker Setup

This repository provides a **Docker Compose configuration** for automatically updating **Cloudflare DNS records** whenever the public IP address changes.  
It ensures continuous domain accessibility, particularly in dynamic IP environments.

## Features
- **Automated DNS record updates** triggered by public IP changes
- **Integration with Cloudflare’s API** for real-time updates
- **Optional Cloudflare proxying** to enhance security and performance
- **Persistent network configuration** using Docker

## Setup Guide

### 1. Configure Environment Variables
Modify the `docker-compose.yml` file to include:
- **API_KEY**: Your **Cloudflare API key**
- **ZONE**: The domain name registered with Cloudflare
- **PROXIED**: Set to `true` to enable Cloudflare’s proxying functionality

### 2. Deploy the Container
Run the following command:
```sh
docker-compose up -d