# Skeleton for Symfony with API Platform on Docker

A modern and robust template for building APIs using Symfony Framework with API Platform, containerized with Docker, and ready for development with Xdebug integration.

## 🚀 Features

- Built on Symfony Framework - Latest stable version
- API Platform integration for easy API development
- Docker containerization for consistent development and deployment
- Xdebug configured and ready to use with Visual Studio Code
- Development and production environment configurations
- PHP web server with Caddy
- Docker Container for suggest client in Next.js
- Docker Container with PostgresSql

## 🛠️ Prerequisites

- Docker and Docker Compose installed
- Visual Studio Code

## ⚙️ Installation

```bash
# Clone the repository
git clone [repository-url]

# Navigate to project directory
cd project-name

# Build the images
docker compose build --no-cache

# Then, start Docker Compose in detached mode to running:
docker compose up --wait
```

## 🔧 Configuration

### Xdebug Setup in VS Code

1. Install the PHP Debug extension in VS Code
2. Add this configuration to your launch.json:

```json
{
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Listen for Xdebug",
            "type": "php",
            "request": "launch",
            "port": 9003,
            "pathMappings": {
                "/var/www/html": "${workspaceRoot}"
            }
        }
    ]
}
```

## 🏃‍♂️ Running the Application

The API Documentation will be available at: [https://localhost](http://localhost:8080)

## 🐳 Docker Services

This skeletonincludes the following services:

- 

## 🔍 Development Features

### Xdebug Integration

Xdebug is configured for:

- Step Debugging
- Error Reporting
- Code Coverage Analysis

### API Platform Features

- Automatic API documentation
- JSON-LD and Hydra support
- OpenAPI (Swagger) specification
- GraphQL support

## 📄 License