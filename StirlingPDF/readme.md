# Stirling PDF Docker Setup  

This repository provides a **Docker Compose configuration** for deploying **Stirling PDF**, a web-based **PDF processing tool** designed for document conversion, editing, and customization.

## Features  
- **Web-based PDF processing** for seamless document management  
- **Integrated OCR (Optical Character Recognition)** using Tesseract training data  
- **Persistent storage** to retain configurations, logs, and custom files  
- **Customizable environment settings** for enhanced security and functionality  

## Container Details  
- **Uses the official Stirling PDF image** (`stirlingtools/stirling-pdf:latest`)  
- **Exposes port `8080`** for web-based document processing  
- **Ensures persistent storage** with the following directories:
  - Training data: `/usr/share/tessdata/`  
  - Extra configurations: `/configs/`  
  - Custom files: `/customFiles/`  
  - Logs: `/logs/`  
- **Environment variables for customization**:
  - `DOCKER_ENABLE_SECURITY`: Enable or disable security settings  
  - `INSTALL_BOOK_AND_ADVANCED_HTML_OPS`: Control additional processing features  
  - `LANGS`: Define the default language  