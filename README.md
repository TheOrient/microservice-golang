# Go Microservices Demo

A multi-service application built with **Go** to explore microservice architecture, service-to-service communication, authentication, logging, messaging, and containerized development.

## Architecture

The repository is organized into several independent services:

- `authentication-service` — authentication and user-related workflows
- `broker-service` — API/broker layer coordinating requests between services
- `listener-service` — background event consumer
- `logger-service` — centralized logging service
- `mail-service` — email-related service
- `front-end` — web-facing application layer
- `project` — orchestration and project-level configuration

## Tech Stack

- Go
- REST APIs
- gRPC / Protocol Buffers
- Docker
- Microservice architecture
- Event-driven communication
- Service-oriented backend design

## What This Project Demonstrates

- Splitting a backend into independently deployable services
- Authentication as a dedicated service
- Inter-service communication
- Background event listeners
- Centralized logging
- Mail-service integration
- API routing through a broker layer
- Containerized local development

## Repository Structure

```text
authentication-service/
broker-service/
front-end/
listener-service/
logger-service/
mail-service/
project/
```

Each service keeps its own Go modules and implementation details so it can be developed and run independently.

## Development Notes

This repository is primarily a learning and architecture project. Before production use, areas such as configuration management, secrets handling, automated testing, observability, CI/CD, service health checks, and deployment strategy should be reviewed and expanded.

## Cleanup Notes

Compiled binaries and operating-system metadata should normally be excluded from source control. A production-quality version of this repository should keep generated binaries and `.DS_Store` files out of Git using `.gitignore`.

## About

This project is part of my backend-development portfolio and focuses on understanding distributed systems and microservice patterns using Go.

Developed by **Ali Gökçe**.
