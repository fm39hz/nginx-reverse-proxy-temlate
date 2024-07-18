# Nginx Reverse proxy template

Small docker script to create nginx reverse proxy

## Preparation

- Create docker network `proxy-net` on target container
- Change domain and email on .env file
- Create .env file

  ```bash
  cp .env.example .env
  ```

## Start proxy

- Start with docker compose

  ```bash
  docker-compose up --build
  ```

- Generate certificate for the first time

  ```bash
  docker exec -it certbot certonly --standalone -d ${DOMAIN_1}
  ```
