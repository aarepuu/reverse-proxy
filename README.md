# reverse-proxy

A simple reverse proxy using Traefik

## Deployment

```bash
# clone repo
git clone https://github.com/aarepuu/reverse-proxy.git && cd reverse-proxy

# create network for traefik
docker network create web

# make a copy of .env variables and edit them (see below for dashboard creds)
cp .env.example .env

# start the proxy
docker-compose up -d
```

## Extras

### Do use default settings for docker logging:

Linux systems

```bash
cp daemon.json /etc/docker/daemon.json
```

Windows

```bash
copy daemon.json C:\ProgramData\docker\config\daemon.json
```

### Set Traefik dashboard user & password:

Use `htpasswd` command line tool to generate basic auth credentials or use `./docker-creds.sh` script (only works on Linux).
