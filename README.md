# Homelab Portfolio – Filip Møldrup Pedersen

## Overview
This homelab is my personal environment for learning real-world IT operations: Linux administration, Docker, networking, DNS, VLANs and security.  
Everything is self-managed – from hardware and OS to services, security and troubleshooting.

## Hardware & OS
- Intel Core i5-7500 + Nvidia GTX 1070
- 28 GB DDR4 RAM
- 500 GB SSD + 1 TB HDD
- Debian-based server with static IP
- 1 Gbit Ethernet via switch into Unifi Express 7

## Network & Domain
- Multiple VLANs on Unifi Express 7
- Static IPs for the server and main desktop
- Public domain: **filippedersen.xyz**
- Subdomain: **mc.filippedersen.xyz** (whitelisted Minecraft Fabric server)
- Other services exposed via Cloudflare DNS and proxy instead of direct home IP

## Services (mostly Docker-based)
- **Jellyfin** media server
- **Minecraft Fabric** server reachable via `mc.filippedersen.xyz` (whitelist only)
- **Python Discord notifier**:
  - Uses Minecraft query
  - Sends notifications when players join/leave
  - Alerts when the server goes down or comes back online
- Additional services running in Docker and proxied via Cloudflare

## Security
- **Fail2ban** on the server and Minecraft service
- Firewall rules limiting exposed ports
- Cloudflare proxy to hide the real home IP
- Whitelisting on the Minecraft server
- VLAN segmentation to reduce blast radius between different device groups

## Skills Demonstrated
- Linux system administration
- Docker containerization and updates
- Networking: VLANs, static IP, DNS, routing, troubleshooting
- Security mindset: least exposure, bans, segmentation
- Scripting and automation with Python
- Structured troubleshooting using logs and network tools

## Why this matters
This setup shows that I can design, run and maintain a small but realistic environment on my own.  
I am used to thinking in terms of uptime, security, and user experience – skills that transfer directly to roles in IT operations, DevOps, infrastructure and support.
