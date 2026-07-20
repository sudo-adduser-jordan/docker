# AGENTS

## Project
Self-hosted developer infrastructure using Docker Compose.

## Services
| Service | Container | Port(s) | Purpose |
|---------|-----------|---------|---------|
| caddy | auto | 80, 443 | Reverse proxy with local TLS |
| adblock | adblock | 53, 1025 | Pi-hole DNS ad blocking |
| git | git | 1026, 222/tcp | Forgejo Git server |
| docker-in-docker | auto | — | DinD for Forgejo CI runners |
| runner | git-runner | — | Forgejo Actions runner |
| postgres | postgres | 5432 | PostgreSQL database |
| pgadmin | pgadmin | 1030 | PostgreSQL management (pgAdmin) |

## Commands
- Start: `docker compose up -d`
- Stop: `docker compose down`
- Logs: `docker compose logs -f <service>`
- Rebuild: `docker compose up -d --build <service>`
- Runner register: `docker exec -it git-runner forgejo-runner register --instance http://10.0.0.5:1026 --token <token> --name "git-runner" --no-interactive`

## Conventions
- Compose file: `docker-compose.yaml`
- Caddy config: `Caddyfile`
- Runner config: `config.yml`
- Env file: `.env` (copy from `.example.env`)
- Networks: all services share the default compose network unless using `network_mode: host`
- Portainer removed — do not add it back
