<p  align="center">

<img  width="300"  src="https://raw.githubusercontent.com/ali-farhad/docker-media-server-offline/main/dmc.jpeg">

</p>

# 📚 About

Docker Media Center is a fully automated media set-up using Jellyfin and a bunch of other services to achieve full automation. All of the services listed below runs locally on your network. This setup allows you to run all services within the same network from docker compose.

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

<b>Clone repository</b><br  />

```

git clone https://github.com/ali-farhad/docker-media-server-offline.git

```

<b>Start docker compose</b><br  />

Inside of `_base/compose` run

```

docker-compose up -d
```

# ⚒️ TODO

- write instructions to connect all services with each other
