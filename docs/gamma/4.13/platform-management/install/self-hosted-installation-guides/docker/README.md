---
description: >-
  Every Gamma component on one host, from MongoDB and Elasticsearch to the
  consoles. Compare the Docker Compose and Docker CLI methods before you start.
---

# Docker

## Deployment methods

Install a fully self-hosted Gamma platform on a single host with one of the following Docker methods.

* [Docker Compose](docker-compose.md)
* [Docker CLI](docker-cli.md)

## Components

Both Docker methods run the same set of containers. The following table lists the Gamma components, their container names, and their published ports.

| Component                      | Container name         | Published port |
| ------------------------------ | ---------------------- | -------------- |
| API Gateway                    | `gamma_gateway`        | `8082`         |
| Management API (Gamma enabled) | `gamma_management_api` | `8083`         |
| APIM Console                   | `gamma_apim_console`   | `8084`         |
| Developer Portal               | `gamma_portal`         | `8085`         |
| Gamma console                  | `gamma_console`        | `8086`         |
| MongoDB                        | `gamma_mongodb`        | n/a            |
| Elasticsearch                  | `gamma_elasticsearch`  | n/a            |
