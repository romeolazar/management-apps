# Home Media Server

LANG=:us:

### Prerequisites.
- A public domain name. Buy one at [https://www.namecheap.com/](https://www.namecheap.com/)
- Use one for free at [https://duckdns.org](https://duckdns.org)
- Docker: [https://docs.docker.com/get-started/](https://docs.docker.com/get-started/)
- Docker Compose: [https://github.com/docker/compose/releases](https://github.com/docker/compose/releases)
- Server platform: [Rocky Linux 8](https://rockylinux.org/download)

# Applications
## management-apps
### [Portainer](https://www.portainer.io/)
Portainer is an open source, platform agnostic tool for managing containerized applications. \
DockerHub: [portainer/portainer](https://hub.docker.com/r/portainer/portainer) \
GitHub: [https://github.com/portainer/portainer](https://github.com/portainer/portainer)

### [FileRun](https://www.filerun.com)
Is a self-Hosted File Sync and Sharing \
DockerHub: [afian/filerun](https://hub.docker.com/r/afian/filerun) \
GitHub:[https://github.com/filerun/docker](https://github.com/filerun/docker)

### [Homepage](https://gethomepage.dev/en/installation/)
A modern (fully static, fast), secure (fully proxied), highly customizable application dashboard with integrations for more than 25 services and translations for over 15 languages. \
GitHub: [benphelps/homepage](https://github.com/benphelps/homepage)

## Info
Because all the services are setup with `docker-compose` they can all reach each other by their Docker Compose service name. So for example when connecting Sonarr with Jacket or qBittorrent, then Jackett would be available on `http://jackett/api....`, which makes everything a lot easier.

### Edit the .env file
All configuration to this setup, I've put in the `.env` file, so all you have to do is go through it and edit it to fit your needs.
