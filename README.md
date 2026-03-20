# RG Platform Orchestration

> **Part of the [ResonantGenesis](https://dev-swat.com) platform** — Master orchestration repo for Docker Compose, deployment scripts, Nginx, and infrastructure configuration.

[![Status: Production](https://img.shields.io/badge/Status-Production-brightgreen.svg)]()
[![Containers: 37](https://img.shields.io/badge/Containers-37-blue.svg)]()
[![License: RG Source Available](https://img.shields.io/badge/License-RG%20Source%20Available-blue.svg)](LICENSE.txt)

## Contents

| Directory | Purpose |
|-----------|---------|
| `docker-compose.unified.yml` | Master compose file for all 37 containers |
| `.env.production.template` | Environment variable template |
| `nginx/` | Nginx configuration |
| `deploy/` | Deployment scripts |
| `docker/` | Docker build configs |
| `scripts/` | Utility and maintenance scripts |
| `cascade_control_plane/` | Service orchestration |
| `performance_tests/` | Load testing |
| `config/` | Shared configuration |
| `contracts/` | Solidity smart contracts |
| `governance/` | RARA governance policies |
| `platform_tools/` | Legacy platform tools reference |

## Usage

This repo replaces the old `genesis2026_production_backend` monolith as the orchestration layer. All service code now lives in individual `RG_*` repos.

```bash
# Deploy all services
cd /home/deploy/RG_Platform_Orchestration
sudo docker compose -f docker-compose.unified.yml up -d --build
```

## Server path
`/home/deploy/RG_Platform_Orchestration`

---
**Organization**: [DevSwat-ResonantGenesis](https://github.com/DevSwat-ResonantGenesis) | **Platform**: [dev-swat.com](https://dev-swat.com)
