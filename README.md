# reverse-proxy
A simple reverse proxy using Traefik



## Deployment

```bash
# clone repo
git clone https://github.com/aarepuu/reverse-proxy.git && cd reverse-proxy

# create network for traefik
docker network create web

# make a copy of .env variables and edit them
cp .env.example .env

# start the proxy
docker-compose up -d
```