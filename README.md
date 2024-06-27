# Multinode Rocket.Chat with MongoDB and Traefik

This project sets up a multinode Rocket.Chat server with a MongoDB database and Traefik as the reverse proxy using Docker Compose. Environment variables are used to make the setup dynamic and easy to configure.

## Prerequisites

- Docker
- Docker Compose

## Getting Started

1. **Clone the repository:**
   ```sh
   git clone https://github.com/SaadatiReza/MultiNode-RocketChat.git
   cd MultiNode-RocketChat
   
2. **Create and configure the .env file:**
   Copy the provided .env.example to .env and adjust the values as needed.
   ```sh
   cp .env-simple .env

3. **Open the .env file and change the variable if needed:**
   Environment Variables:
   Key attributes brought into the .env file include:
   
   TRAEFIK_IMAGE: The Traefik image to use.
   ROCKETCHAT_IMAGE: The Rocket.Chat image to use.
   MONGO_IMAGE: The MongoDB image to use.
   ROOT_URL: The root URL for Rocket.Chat.
   ROCKET_REPLICAS: Number of Rocket.Chat instances.
   TRAEFIK_API_PORT: Port for the Traefik API dashboard.
   TRAEFIK_HTTP_PORT: HTTP port for Traefik.
   TRAEFIK_HTTPS_PORT: HTTPS port for Traefik.
   ROCKETCHAT_PORT: Port for Rocket.Chat.
   MONGO_PORT: Port for MongoDB.

4. **Run the services:**
   ```sh
   docker compose up -d

