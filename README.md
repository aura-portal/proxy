# Proxy

## Details

This is intended for local use only to replicate a simple load balancer.

## Usage

```yaml
# docker-compose.yaml
---
services:
  proxy:
    image: ghcr.io/aura-portal/proxy:v0
    ports:
      - 80:80
  # core and module config
```
