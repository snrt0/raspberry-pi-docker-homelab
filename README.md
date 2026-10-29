# Raspberry Pi 5 Docker 

## Project Overview

This project documents my experience deploying and managing self-hosted services using Docker on Raspberry Pi OS. 
## Hardware and Software

- Raspberry Pi 5 (4GB RAM)
- Raspberry Pi OS (64-bit)
- High-pi Pro 5S case
- Docker
- UptimeKuma
- SSH
- Void Linux ThinkPad T480 (administration workstation)

## Architecture

```text
Void Linux ThinkPad
       |
       | SSH
       v
 Raspberry Pi 5
       |
       v
     Docker
       |
       v
   Uptime Kuma
       |
       v
 Router monitoring
```

## Implemented Features

### Remote Administration
- Configured headless Raspberry Pi OS
- Enabled SSH for remote administration
- Accessed the Raspberry Pi from a Linux workstation

### Containerization
- Installed Docker
- Deployed Uptime Kuma as a container
- Configured container port mapping
- Verified access to the monitoring dashboard

### Network Monitoring
- Configured Uptime Kuma to monitor router availability
- Verified connectivity and monitored uptime
## Screenshots

### UptimeKuma monitoring dashboard

The dashboard displays the availability and uptime of my home router

![Uptime Kuma Dashboard](Screenshots/uptimekuma.png)

## Troubleshooting

During deployment, I investigated browser connection failures, container status, and incorrect port configurations. I corrected the Docker port mapping and successfully accessed Uptime Kuma through its web interface.


- [x] Configure Raspberry Pi OS
- [x] Enable SSH
- [x] Install Docker
- [x] Deploy UptimeKuma
- [x] Monitor router availability 

