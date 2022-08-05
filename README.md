# My Proxmox Setup

All the services I'm running on my Proxmox instance.

## Table of Contents

- Setup

	- [Remote Development Server Setup](https://github.com/SushritPasupuleti/Proxmox-Remote-Development-Server-Setup)

	- [GPU Passthrough](https://github.com/SushritPasupuleti/Proxmox-GPU-Sharing-Passthrough)

	- [Docker Setup](https://github.com/SushritPasupuleti/Proxmox-Docker-Setup)

- Apps

	- [Pihole](#pihole)

	- [Nginx Proxy Manager](#nginx-proxy-manager)

	- [n8n](#n8n)

### Pihole

Block all tracking and ads over your entire network. Basic setup [here](https://github.com/SushritPasupuleti/Pihole-with-Proxmox)

### [Nginx Proxy Manager](https://nginxproxymanager.com/guide/#features)

Essential for all internal networking.

### [n8n](https://docs.n8n.io/hosting/installation/docker/)

For workflow automation

Run with:

```bash
docker run -it --rm \
    --name n8n \
    -p 5678:5678 \
    -v ~/.n8n:/home/node/.n8n \
    n8nio/n8n
```

Data is persisted to `.n8n`

