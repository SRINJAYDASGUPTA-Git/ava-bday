# Deploy Avanti — A Little Universe with Docker

This project builds the Astro site into static HTML/CSS/JS and serves it with Nginx.
The deployment container does not need Node.js at runtime.

## Build and run locally

```bash
docker compose up -d --build
```

Open http://localhost:8088. To use a different host port, create `.env` with:

```env
AVANTI_PORT=8090
```

Then recreate the service:

```bash
docker compose up -d --build
```

## Deploy to your server

Copy the project directory to the server (or clone your Git repository), then run:

```bash
cd avanti-universe
docker compose up -d --build
```

The site will be available at `http://SERVER-IP:8088` by default. If your server already has a reverse proxy (Nginx Proxy Manager, Traefik, Caddy, etc.), proxy your chosen hostname to the container at `avanti-universe:80` on the same Docker network, or to `SERVER-IP:8088` from the host.

## Update after changing the site

Copy/pull the updated source and run:

```bash
docker compose up -d --build
```

## Useful commands

```bash
docker compose logs -f
docker compose ps
docker compose down
```
