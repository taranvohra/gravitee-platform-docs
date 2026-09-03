---
description: >-
  A hybrid Gateway on one host talks to a Gravitee Cloud control plane. Compare
  the Docker Compose and Docker CLI methods and what each one runs.
---

# Docker

## Deployment methods

Deploy a hybrid Gamma Gateway on a single host with one of the following Docker methods.

* [Docker Compose](docker-compose.md)
* [Docker CLI](docker-cli.md)

## Components

A hybrid Docker deployment runs the data plane only. The following table lists the containers, their names, and their published ports.

| Component             | Container name             | Published port |
| --------------------- | -------------------------- | -------------- |
| API Gateway           | `gio_gamma_hybrid_gateway` | `8082`         |
| Redis (rate limiting) | `gio_gamma_hybrid_redis`   | `6379`         |
