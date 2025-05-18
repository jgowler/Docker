# Docker Installation & Uninstallation Guide

This repository provides scripts for the **installation and removal of Docker**, ensuring a smooth setup and complete uninstallation while maintaining system integrity.

## Docker Installation

The installation script configures **Docker Engine, CLI, container runtime, and Docker Compose** on a Linux system.

### Features
- **Secure installation** with official GPG key verification
- **Adds Docker repository sources** for automatic updates
- **Installs essential Docker components** for containerized environments
- **Creates a test container** (`hello-world`) for verification
- **Adds the current user to the `docker` group** for seamless permission management

### Why Use This Script?
- Automates setup, minimizing manual configuration
- Ensures **Docker and required dependencies** are properly installed
- Provides **user-friendly access control** for efficient management

---

## Docker Uninstallation

The removal script **thoroughly purges Docker**, ensuring no residual data remains after removal.

### Features
- **Removes all Docker packages**, including CLI and runtime dependencies
- **Deletes stored images, containers, and volumes** to prevent leftover data
- **Cleans up repository sources and security keys** for a complete uninstallation