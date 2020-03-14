# ago-assistant
Runs ESRI "AGO Assistant" in a Docker container.

## Prerequisites 

* A server that has Docker and optionally Docker Compose installed.

## Build image

```bash
docker-compose build
```
### Deployment

The docker-compose.yml is set up to use Wildsong/docker-proxy as a web proxy
and the proxy will create Let's Encrypt certificates. To get that to work,

*Set up a host name for example I use "agoa.wildsong.biz"
*Set up an app id in your portal
*Copy sample.env to .env
*Edit .env to pu the host name, app id, and hostname of your Portal in it.

```bash
docker-compose up -d
```

Runs on port 80 by default, you can change the in docker-compose.yml




