# Home Media Server

LANG=:us:

### Prerequisites.
- A public domain name. Buy one at [https://www.namecheap.com/](https://www.namecheap.com/)
- Use one for free at [https://duckdns.org](https://duckdns.org)
- Docker: [https://docs.docker.com/get-started/](https://docs.docker.com/get-started/)
- Docker Compose: [https://github.com/docker/compose/releases](https://github.com/docker/compose/releases)
- Server platform: [Rocky Linux 8](https://rockylinux.org/download)

# Applications
## media-apps
### [Radarr](https://radarr.video/)
Radarr is an independent fork of Sonarr reworked for automatically downloading movies via Usenet and BitTorrent. \
DockerHub: [linuxserver/radarr](https://hub.docker.com/r/linuxserver/radarr/) \
GitHub: [linuxserver/docker-radarr](https://github.com/linuxserver/docker-radarr)

### [Sonarr](https://sonarr.tv/)
Sonarr is a PVR for Usenet and BitTorrent users. It can monitor multiple RSS feeds for new episodes of your favorite shows and will grab, sort and rename them. It can also be configured to automatically upgrade the quality of files already downloaded when a better quality format becomes available. \
DockerHub: [linuxserver/sonarr](https://hub.docker.com/r/linuxserver/sonarr/) \
Github: [linuxserver/docker-sonarr](https://github.com/linuxserver/docker-sonarr)

### [Lidarr](https://lidarr.audio)
It can monitor multiple RSS feeds for new albums from your favorite artists and will interface with clients and indexers to grab, sort, and rename them. \
DockerHub: [linuxserver/lidarr](https://hub.docker.com/r/linuxserver/lidarr) \
GitHub: [linuxserver/docker-lidarr](https://github.com/linuxserver/docker-lidarr)

### [Bazarr](https://www.bazarr.media)
Is a companion application to Sonarr and Radarr. It manages and downloads subtitles based on your requirements. You define your preferences by TV show or movie and Bazarr takes care of everything for you. \
DockerHub: [linuxserver/bazarr](https://hub.docker.com/r/linuxserver/bazarr) \
GitHub: [morpheus65535/bazarr](https://github.com/morpheus65535/bazarr)

### [Jackett](https://github.com/Jackett/Jackett)
Jackett works as a proxy server: it translates queries from apps (Sonarr, Radarr, Lidarr, qBittorrent, etc) into tracker-site-specific http queries, parses the html response, then sends results back to the requesting software. This allows for getting recent uploads (like RSS) and performing searches. \
DokcerHub: [linuxserver/jackett](https://hub.docker.com/r/linuxserver/jackett/) \
Github: [linuxserver/docker-jackett](https://github.com/linuxserver/docker-jackett)

### [Prowlarr](https://github.com/Prowlarr/Prowlarr)
Prowlarr is an indexer manager/proxy built on the popular *arr .net/reactjs base stack to integrate with your various PVR apps. \
DockerHub: [linuxserver/prowlarr](https://hub.docker.com/r/linuxserver/prowlarr) \
GitHub: [prowlarr/prowlarr](https://github.com/Prowlarr/Prowlarr)

### [Plex](https://www.plex.tv/)
Plex media server allows you to aggregate all your personal media and access it anywhere you go. Enjoy your own content on all your devices with Plex. \
DockerHub: [plexinc/pms-docker](https://hub.docker.com/r/plexinc/pms-docker/) \
Github: [plexinc/pms-docker](https://github.com/plexinc/pms-docker)

### [qBittorrent](https://www.qbittorrent.org)
Is an advanced and multi-platform BitTorrent client. \
DockerHub:[linuxserver/qbittorrent](https://hub.docker.com/r/linuxserver/qbittorrent) \
GitHub: [linuxserver/docker-qbittorrent](https://github.com/linuxserver/docker-qbittorrent)

## Info
Because all the services are setup with `docker-compose` they can all reach each other by their Docker Compose service name. So for example when connecting Sonarr with Jacket or qBittorrent, then Jackett would be available on `http://jackett/api....`, which makes everything a lot easier.

### Edit the .env file
All configuration to this setup, I've put in the `.env` file, so all you have to do is go through it and edit it to fit your needs.
