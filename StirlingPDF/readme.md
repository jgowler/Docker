# 📄 Stirling PDF Docker Setup  

A **Docker Compose configuration** for deploying **Stirling PDF**, a versatile web-based **PDF processing tool**.  
This setup allows for **document conversion, editing**, and **custom configurations**.

## 🚀 Features  
- **Process PDFs directly in the browser**  
- **Supports OCR (Optical Character Recognition)** via Tesseract training data  
- **Persistent storage** for configurations, logs, and custom files  
- **Customizable environment settings** for security and functionality  

## 🔧 Container Details  
- **Runs the official Stirling PDF image** (`stirlingtools/stirling-pdf:latest`)  
- **Exposes port `8080`** for web-based document processing  
- **Persistent storage locations**:
  - Training data (`/usr/share/tessdata/`)  
  - Extra configs (`/configs/`)  
  - Custom files (`/customFiles/`)  
  - Logs (`/logs/`)  
- **Environment variables for customization**:
  - `DOCKER_ENABLE_SECURITY`: Disable/enable security settings  
  - `INSTALL_BOOK_AND_ADVANCED_HTML_OPS`: Control additional processing features  
  - `LANGS`: Set default language