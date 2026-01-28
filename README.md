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
```

---

For clients
-----------

Once this toolkit is deployed on your server, you will typically get:

- One URL for everything, for example: `http://your-server/`
- Simple paths for each tool:
  - Passwords: `http://your-server/passwords`
  - Helpdesk: `http://your-server/tickets`
  - File sync: `http://your-server/files`
  - PDF tools: `http://your-server/pdf`
- A single IT contact (your MSP/IT partner) who manages backups, updates, and access for all tools.

Ask your IT partner for:
- Your toolkit URL
- Who can access which tool
- How backups and password recovery are handled

