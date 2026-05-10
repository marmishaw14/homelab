# 🏠 My Homelab

> Self-hosted infrastructure powering my projects, APIs, and experiments in distributed systems, DevOps, and backend development.

---

## 📌 Table of Contents
- [Overview](#-overview)
- [Architecture](#-architecture)
- [Services](#-services)
- [Hardware](#-hardware)
- [What I'm Looking to Add Next](#-what-im-looking-to-add-next)

---

## 🧠 Overview
This homelab is a **self-hosted environment** where I deploy and manage applications using modern DevOps practices.

**Goals:**
- Learn real-world infrastructure (Docker, networking, monitoring)
- Host personal + portfolio projects
- Experiment with distributed systems & AI workloads
- Build production-like backend systems

---

## 🏗️ Architecture
How my homelab services interact with each other.

```text
                ┌────────────────────────────┐
                │        Cloudflare          │
                │   DNS + Tunnel + HTTPS     │
                └────────────┬───────────────┘
                             │
                             ▼
                   ┌───────────────────┐
                   │  Ubuntu Server    │
                   │     "abyss"       │
                   └─────────┬─────────┘
                             │
                             ▼
                   ┌───────────────────┐
                   │ Docker + Compose  │
                   └─────────┬─────────┘
                             │
        ┌────────────────────┼────────────────────┐
        ▼                    ▼                    ▼
┌───────────────┐    ┌────────────────┐   ┌────────────────┐
│  App Services │    │  Monitoring    │   │  AI / Tools    │
│ Node APIs     │    │ Beszel/Grafana │   │ Ollama/etc.    │
└───────────────┘    └────────────────┘   └────────────────┘
```

---

## 🚀 Services

| Service(s) | Description |
|--------|------------|
| Grafana, Beszel | Grafana for dashboards, Beszel for lightweight server monitoring |
| Cloudflared | Connector that lets local apps be reachable from the internet without opening ports |
| Portainer | GUI for managing my Docker containers |
| Vaultwarden | Self-hosted alternative to Bitwarden for secrets and password management | 
---
## 💻 Hardware
I'm running Ubuntu Server headless on an old PC that's running 24/7 in my basement.
| Hardware | Details |
|--------|------------|
| **OS** | Ubuntu Server 24.04.4 LTS |
| **CPU** | AMD FX(tm)-6300 Six-Core Processor |
| **RAM** | 8GB (I know it's low... I'm using an old PC) |

## 🤔 What I'm Looking to Add Next
Some services I'm looking to self-host next are Immich for photo and video management, and Plex for media sharing. I'm always looking to add new services on my homelab to make my life easier, while also having control and privacy over my data.
