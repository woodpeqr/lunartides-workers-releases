# LunarTides Worker Services — Releases

This repository contains pre-compiled binaries for the LunarTides worker services
(flux, rift, swell, shoal). Source code is private.

## Available workers

| Worker | Endpoint | Role |
|--------|----------|------|
| `flux` | `POST /validate` | Contact validator |
| `rift` | `POST /enrich` | Contact enricher |
| `swell` | `POST /score` | Contact scorer |
| `shoal` | `POST /tag` | Contact tagger (bonus) |

## Installation

Workers are distributed as Docker images in the workshop's `docker-compose.yml`.
To download a binary directly:

```bash
curl -fsSL https://github.com/woodpeqr/lunartides-workers-releases/releases/download/v0.1.0/flux_linux_amd64 -o flux
chmod +x flux
```

## Pre-session smoke test

```bash
curl -fsSL https://github.com/woodpeqr/lunartides-workers-releases/releases/download/v0.1.0/flux_linux_amd64 -o /dev/null && echo "OK"
```
