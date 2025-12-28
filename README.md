# Confiance Platform - Infrastructure

Infrastructure and deployment configurations for the Confiance Financial Platform.

## Contents

- `docker-compose.yml` - Local development setup
- `docker-compose.prod.yml` - Production deployment setup
- `.env.template` - Environment variables template

## Quick Start

### Local Development
```bash
# Copy environment template
cp .env.template .env

# Edit .env with your values
nano .env

# Start all services
docker-compose up -d

# Check status
docker-compose ps

# View logs
docker-compose logs -f
```

### Production Deployment

See [DEPLOYMENT_GUIDE.md](../docs/DEPLOYMENT_GUIDE.md) for detailed instructions.

## Services

- **discovery-service** (8761) - Eureka service registry
- **api-gateway** (8080) - API Gateway
- **auth-service** (8081) - Authentication
- **user-service** (8082) - User management
- **investment-service** (8084) - Investment products
- **transaction-service** (8085) - Transactions
- **portfolio-service** (8086) - Portfolio management
- **notification-service** (8083) - Email notifications
- **mysql** (3306) - Database
- **redis** (6379) - Cache

## Documentation

- [API Documentation](https://github.com/confiance-platform)
- [Architecture](https://github.com/confiance-platform)
- [Deployment Guide](https://github.com/confiance-platform)

## License

Proprietary - Confiance Financial Platform
