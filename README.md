# Nginx Reverse proxy template

Small docker script to create nginx reverse proxy

## Preparation

- Create docker network `proxy-net` on target container
- Change domain and email on .env file
- Create .env file

  ```bash
  mv .env.example .env
  ```

## Start proxy

- Start with docker compose

  ```bash
  docker-compose up --build
  ```
