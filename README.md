<p  align="center">

<img  width="500"  src="https://raw.githubusercontent.com/BeefBytes/Assets/master/Other/container_illustration/v2/dmc.png">

</p>

# 📚 About

Docker Media Center is a fully automated media set-up using Jellyfin and a bunch of other services to achieve full automation. All of the services listed below are running behind Traefik reverse proxy with proper certificates and basic auth. This script allows you to run all services within the same network from docker compose

Furthermore, the guide is set up with volume paths in a way to allow hardlinks of media files rather than making copies. This means once a media file is downloaded, it is hardlinked to the Jellyfin media directory rather than copied. Such a method is faster and saves storage on your server.

### Services

- Jellyfin

- Transmission

- Radarr

- Sonarr

- Prowlarr

- Jellyseerr

# 🧰 Getting Started

This guide assumes you have a basic knowledge of linux and Docker / Docker Compose.

### Requirements

- [Docker](https://docs.docker.com/engine/install/ubuntu/)

# 🏗️ Installation

## Preparations

First we want configure enviroment variables and setup domain records before installing anything.

<b>Clone repository</b><br  />

```

git clone

```

<b>Start docker compose</b><br  />

Inside of `_base/compose` run

```

docker-compose up -d
```

# ⚒️ TODO

- write instructions to connect all services with each other
