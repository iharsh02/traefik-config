# Traefik Reverse Proxy with Docker Compose

This repository contains a configuration for setting up Traefik as a reverse proxy using Docker Compose. Traefik is configured to use Cloudflare for DNS challenge and Let's Encrypt for SSL certificates.

## Prerequisites

- Docker
- Docker Compose

## Setup

1. **Clone the repository**:
   ```sh
   git clone <repository-url>
   cd <repository-directory>
   ```


2. **Create a .env file: Create a .env file in the root directory of the project and add your Cloudflare API token:**
  ```sh
   CF_DNS_API_TOKEN=your-cloudflare-dns-api-token
  ```
3. **Set permissions for the certificates directory:**

    ```sh
    sudo chmod 600 data/certs
    ```
4. **Start the services:**
    ```sh
    docker compose up 
    ```

_Accessing the Dashboard at port 8080_