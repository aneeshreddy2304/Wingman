<p align="center"><img src="docs/assets/banner.svg" alt="Wingman — Connect stranded drivers with nearby help." width="100%"></p>

<p align="center"><img src="docs/assets/badges/react.svg" alt="react" height="28"> <img src="docs/assets/badges/fastapi.svg" alt="fastapi" height="28"> <img src="docs/assets/badges/postgresql.svg" alt="postgresql" height="28"> <img src="docs/assets/badges/postgis.svg" alt="postgis" height="28"> <img src="docs/assets/badges/sqlalchemy.svg" alt="sqlalchemy" height="28"> <img src="docs/assets/badges/docker.svg" alt="docker" height="28"></p>

<p align="center"><strong>A full-stack roadside-assistance marketplace for service requests, nearby mechanics, inventory, messaging, and job coordination.</strong></p>

## Overview

A full-stack roadside-assistance marketplace for service requests, nearby mechanics, inventory, messaging, and job coordination.

### Why it matters

Wingman brings the fragmented roadside-help journey into one location-aware workspace for drivers, mechanics, and parts providers.

## Key features

- Role-based driver and mechanic workflows
- PostGIS-powered nearby service discovery
- Service-request lifecycle and messaging
- Parts marketplace and warehouse inventory

## Architecture

```mermaid
flowchart LR
  A[React web app] --> B[FastAPI]
  B --> C[(PostgreSQL + PostGIS)]
  B --> D[Auth + role workflows]
  B --> E[Requests + messages]
  B --> F[Parts marketplace]
```

## Technology stack

**react** · **fastapi** · **postgresql** · **postgis** · **sqlalchemy** · **docker**

## Getting started

Configure `backend/.env` and `frontend/.env.local` from the examples, initialize a disposable PostgreSQL/PostGIS database, start FastAPI, then run the Vite frontend. Use synthetic records for demos.
