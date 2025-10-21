# MediaWiki Docker Setup

A lightweight and portable **MediaWiki** environment for local or self-hosted deployments.  
Includes MySQL, MediaWiki, and simple configuration templates for clean, reproducible setup.

---
##  Structure
```bash
mediawiki-docker/
├── docker-compose.yml
├── .env.example
├── localsettings/
│ └── LocalSettings.php.template
└── backups_config/
```
---

## Quick Start

1. Copy `.env.example` to `.env` and configure it:
   ```bash
   cp .env.example .env

Update the database credentials and MediaWiki settings inside .env.

2. Start the stack:
```bash
docker-compose up -d
```

3. Open your browser and go to:
```
http://localhost:8080
```

or the corresponding host where Docker is running.

🔒 Secrets

Sensitive data such as database passwords, API keys, and MediaWiki secret keys are not included in this repository.
Use the .env file (excluded from version control) to store them locally.

Backup & Restore

This project includes an optional backup configuration under backups_config/.
These files are ignored by Git and meant for local use only.

Notes

Default skin: vector-2022

PHP and MediaWiki versions can be adjusted in docker-compose.yml

Recommended for personal or development use



MIT License © 2025 Arsen Jijavadze

