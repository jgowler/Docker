# Prometheus & Grafana Docker Setup  

🚧 **Work in Progress** – Not yet ready for deployment 🚧  

This repository provides a **Docker Compose configuration** for deploying **Prometheus** to collect metrics and **Grafana** to visualize them.  
The setup ensures **persistent storage**, basic security configurations, and a seamless monitoring environment.

## Features  

### Grafana  
- **Advanced visualization tool** for monitoring and analytics  
- **Accessible via port `3000`** for dashboards and reporting  
- **Persistent storage** maintained in the `grafana-data` volume  
- **Configurable admin security settings** via environment variables  

### Prometheus  
- **Collects and stores system and application metrics**  
- **Customizable configuration** via `prometheus.yaml`  
- **Exposes port `9090`** for metric queries and monitoring  
- **Ensures persistent data storage** using the `prometheus-data` volume  
- **Auto-restarts** for high availability  

## Deployment Guide  

### 1. Modify Environment Variables *(optional)*  
- Set `GF_SECURITY_ADMIN_PASSWORD` for Grafana admin access  
- Ensure `prometheus.yaml` is properly configured  

### 2. Deploy the Containers  
Execute the following command:  
```sh
docker-compose up -d