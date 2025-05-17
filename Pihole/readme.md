# 🚫 Pi-hole Docker Setup  

A **Docker Compose configuration** to deploy **Pi-hole**, a powerful **network-wide ad blocker** that filters unwanted ads and trackers at the DNS level.  
This setup ensures **persistent storage**, customizable configurations, and optional DHCP support.

## 🚀 Features  
- **Network-wide ad blocking** at the DNS level  
- **Customizable DNS settings** with a web interface  
- **Supports DHCP server mode** *(optional)*  
- **HTTPS access** with a self-signed certificate  
- **Persistent storage** for configuration and logs  

## 🔧 Container Details  
- **Runs the official Pi-hole image** (`pihole/pihole:latest`)  
- **Exposes essential ports** for network functionality:
  - `53`: DNS resolution (TCP/UDP)  
  - `80`: Web interface  
  - `443`: Secure HTTPS access *(self-signed certificate)*  
  - *(Optional)* `67`: DHCP server  
  - *(Optional)* `123`: NTP server  
- **Stores configuration files** in `/Pi-Hole-Data/` volume for persistence  
- **Supports custom `dnsmasq` settings** for advanced configurations  

## ⚙️ Deployment Guide  

1️⃣ **Prepare the Environment**  
- Place the `docker-compose.yml` file in a directory on your Docker host  
- *(Optional)* Modify environment variables for timezone, password, and DNS settings  

2️⃣ **Deploy the Container**  
Run the following command:  
```sh
docker-compose up -d
