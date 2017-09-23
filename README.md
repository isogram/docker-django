# Docker Shankly

## Introduction
Docker Shankly is a docker stack for Django Framework

## What's Included
- Django Framework v1.11.5
- Postgres
- Redis
- Nginx
- Gunicorn

## How To
- Make sure Docker is installed on your system
- Clone repo
- `docker-compose build` (Wait and you can take a coffe. It depends on your connection speed)
- `docker-compose up`

# Key Points
1. Configuration like db name, db password is located in `env` file
2. Your main working docker container is `shankly-web`  
   Explore it via `docker exec -it shankly-web sh`
3. Postgres data will be stored at `postgres/data`
4. Your main working directory is `web/app`
5. Feel free to customize the `Dockerfile` and `docker-compose.yaml` . Don't forget to rebuild after it.