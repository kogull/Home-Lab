# Home Lab Setup

This repository documents the setup and configuration of my home lab environment using Proxmox. The lab includes a TrueNAS storage solution, Jellyfin media server, Docker with Portainer for container management, and a Minecraft server hosted through Portainer.

## Table of Contents

- [Overview](#overview)
- [Technologies Used](#technologies-used)
- [Setup Guide](#setup-guide)
  - [1. Proxmox Installation](#1-proxmox-installation)
  - [2. TrueNAS Installation](#2-truenas-installation)
  - [3. Jellyfin Setup](#3-jellyfin-setup)
  - [4. Docker & Portainer Setup](#4-docker--portainer-setup)
  - [5. Minecraft Server Deployment](#5-minecraft-server-deployment)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project is a guide to building a robust home lab environment. Using Proxmox as the virtualization platform, I've set up TrueNAS for network-attached storage, Jellyfin for media streaming, Docker and Portainer for container management, and a Minecraft server.

## Technologies Used

- **Proxmox VE**: Virtualization platform
- **TrueNAS**: Network-attached storage
- **Jellyfin**: Media server
- **Docker**: Containerization platform
- **Portainer**: Docker management UI
- **Minecraft**: Game server hosted within Docker

## Setup Guide

### 1. Proxmox Installation

1. Download the Proxmox VE ISO from the [official website](https://www.proxmox.com/en/downloads).
2. Create a bootable USB drive and install Proxmox on your server hardware.
3. Access the Proxmox web interface via `https://your-server-ip:8006` and log in.

### 2. TrueNAS Installation

1. **Create a new VM in Proxmox:**
   - Allocate resources (e.g., 4 CPUs, 8GB RAM, 100GB storage).
   - Mount the TrueNAS ISO as the installation medium.

2. **Install TrueNAS:**
   - Boot the VM and follow the installation prompts.
   - Configure your storage pools and shares.

3. **Configure network and storage:**
   - Set up your network interfaces and assign IP addresses.
   - Create datasets for different types of data (e.g., media, backups).

### 3. Jellyfin Setup

1. **Create a Docker container for Jellyfin:**

   Install Docker if it's not already installed:
   ```bash
   sudo apt update
   sudo apt install docker.io
   sudo systemctl start docker
   sudo systemctl enable docker