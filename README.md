# The Address Apartments Project

## Project Overview
A full-stack application for apartment management with:
- Frontend: Next.js web application
- Backend: NestJS REST API
- PostgreSQL database

## Prerequisites
- Docker 20.10+
- Docker Compose 2.20+

## Quick Start with Docker
```bash
# Clone the project
git clone https://github.com/yourusername/the-address-apartments-project.git
cd the-address-apartments-project

# Build and start all services
docker compose up --build -d

# Access applications:
- Frontend: http://localhost:3000
- Backend API: http://localhost:8080
```

## Environment Configuration
### Required Environment Variables
```
POSTGRES_USER=postgres
POSTGRES_PASSWORD=password
POSTGRES_DB=address_apartments
```

## Service Ports
| Service      | Port |
|--------------|------|
| Frontend     | 3000 |
| Backend API  | 8080 |
| PostgreSQL   | 5433 |

## Development Workflow
```bash
# Stop all containers
docker compose down

# Rebuild specific service
docker compose up --build -d frontend

# View logs
docker compose logs -f backend
```

## Project Structure
```
├── frontend/      # Next.js application
├── backend/       # NestJS API
└── docker-compose.yml # Main deployment configuration
```