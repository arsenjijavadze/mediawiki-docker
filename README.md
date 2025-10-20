# MediaWiki Docker — DevOps-Wiki

Local MediaWiki deployment using docker-compose (MediaWiki + MariaDB).
This repository contains the compose scaffold and templates only — **no secrets**.

## Quickstart
1. Copy `.env.example` to `.env` and fill credentials.
2. Start: `docker compose up -d`
3. Admin UI: `http://server-03-vm:8080`

## Notes
- LocalSettings.php is not stored in repo. See `localsettings/LocalSettings.php.template`.
- Backups, dumps and .env are ignored via `.gitignore`.
