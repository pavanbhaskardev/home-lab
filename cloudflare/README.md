# Cloudflare tunnel (cloudflared)

It's a tunneling daemon that proxies traffic from the Cloudflare network to your origins. This directory contains docker-compose setup of cloudflare tunnels

Official Github Repo: https://github.com/cloudflare/cloudflared

### Step 1

- Create a docker network called cloudflare

```bash
docker network create cloudflare
```

### Step 2

- Create a `.env` file by taking `.env.example` as reference.
- Paste your `CLOUDFLARE_TUNNEL_TOKEN` in .env.
- Start the docker compose setup

```bash
docker compose up -d
```
