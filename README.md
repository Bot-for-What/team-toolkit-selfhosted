# team-toolkit-selfhosted
# Team Toolkit (Self-Hosted, Docker)

Production-ready Docker stack that gives small teams four essential internal tools on their own server:

- **Vaultwarden** – Team Password Manager (`/passwords`)
- **osTicket** – Helpdesk & Ticketing (`/tickets`)
- **Syncthing** – File Sync & Backup GUI (`/files`)
- **BentoPDF** – PDF Utilities (`/pdf`)

All apps run behind **Caddy** as a reverse proxy, exposed on simple paths on port 80.

---

## What this is for

This stack is designed for:

- Small clinics, offices, agencies, schools
- Teams that currently use Excel/WhatsApp for passwords, requests, and files
- Anyone who wants a simple, self-hosted “internal toolkit” without complex setup

You can deploy this on:

- A client’s on-prem Server
- A cheap VPS (Hetzner, AWS Lightsail, etc.)

---

## Quick start (local or server)

Prerequisites:

- Docker
- Docker Compose (or `docker compose` plugin)

```bash
git clone https://github.com/bot-for-what/team-toolkit-selfhosted.git
cd team-toolkit-selfhosted

docker compose up -d

