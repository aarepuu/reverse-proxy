# reverse-proxy
A simple reverse proxy using Traefik

# deployment

```bash
# clone repo
git clone https://github.com/aarepuu/reverse-proxy.git && cd reverse-proxy

# make a copy of .env variables and edit them
cp .env.example .env

# start the proxy
docker-compose up -d

```