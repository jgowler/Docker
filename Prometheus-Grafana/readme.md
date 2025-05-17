# 📊 Prometheus & Grafana Docker Setup  

🚧 **Work in Progress** – Not yet ready for deployment 🚧  

A **Docker Compose configuration** to deploy **Prometheus** for collecting metrics and **Grafana** for visualizing them.  
This setup provides persistent storage and basic security configurations for monitoring environments.

## 🚀 Features  

### 📈 Grafana  
- **Powerful visualization tool** for monitoring data  
- **Accessible via port `3000`** for dashboards and analytics  
- **Persistent storage** for settings in `grafana-data` volume  
- **Admin security settings configurable** via environment variables  

### 🔍 Prometheus  
- **Collects system and application metrics**  
- **Configurable via `prometheus.yaml`**  
- **Exposes port `9090`** for metric queries and monitoring  
- **Persistent data storage** in `prometheus-data` volume  
- **Auto-restarts to ensure availability**  

## ⚙️ Deployment Guide  

1️⃣ **Modify Environment Variables** *(optional)*  
- Set `GF_SECURITY_ADMIN_PASSWORD` for Grafana admin access  
- Ensure `prometheus.yaml` is configured properly  

2️⃣ **Deploy the Containers**  
Run the following command:  
```sh
docker-compose up -d
