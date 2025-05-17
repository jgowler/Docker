# 🌍 Cloudflare Dynamic DNS (DDNS) Docker Setup  

A **Docker Compose configuration** to automatically update **Cloudflare DNS records** when your **public IP address changes**.  
This ensures seamless domain access, especially for dynamic IP environments.

## 🚀 Features  
- **Automatically updates DNS records** when the public IP changes  
- **Uses Cloudflare's API** for instant updates  
- **Supports proxying** through Cloudflare for enhanced security  
- **Persistent network configuration** using Docker  

## 🔧 Setup Guide  

### 1️⃣ Configure Environment Variables  
Edit the `docker-compose.yml` file to include:  
- **API_KEY:** Your **Cloudflare API key**  
- **ZONE:** The domain name linked to Cloudflare  
- **PROXIED:** Set to `true` to use Cloudflare's proxy  

### 2️⃣ Deploy the Container  
Run the following command:  
```sh
docker-compose up -d
