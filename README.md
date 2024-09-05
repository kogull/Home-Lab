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
  - [5. Minecraft Server Deployment](#5-game-server)

## Overview

This project is a guide to building a robust home lab environment. Using Proxmox as the virtualisation platform, I've set up TrueNAS for network-attached storage, Jellyfin for media streaming, Docker and Portainer for container management, and a Minecraft server.

## Technologies Used

- **Proxmox VE**: Virtualisation platform
- **TrueNAS**: Network-attached storage
- **Jellyfin**: Media server
- **Docker**: Containerisation platform
- **Portainer**: Docker management UI
- **Minecraft**: Game server hosted within Docker

## Setup Guide

### 1. Proxmox Installation
- Download and installed Proxomox onto an old computer I had 
- Accessed the Proxmox through web interface

### 2. TrueNAS Installation
1. **Create a new VM in Proxmox**
2. **Install TrueNAS:**
3. **Configured storage:**
   - Create datasets for different types of data (e.g., media, backups)
   - Create accounts different types of access

### 3. Jellyfin Installation
1. **Create a new VM in Proxmox**
2. **Install Jellyfin:**
3. **Configure:**
   - Connect TrueNas storage
   - Add media and files

### 4. Docker Portainer  Installation
1. **Create a new Container in Proxmox**
2. **Install Ubuntu Server:**
3. **Configure:**
   - SSH into server and install Docker
4. **Portainer**
   - Install as container in docker
   - Launch the and manage through web UI

### 5. Game Server
1. **Create a new Container in Portainer**
   - Configure port for access
3. **Connect to the server**
