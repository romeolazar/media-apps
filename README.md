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

## smarthome-apps
### [Homebridge](https://homebridge.io)
Homebridge allows you to integrate with smart home devices that do not natively support HomeKit. There are over 2,000 Homebridge plugins supporting thousands of different smart accessories. \
DockerHub: [oznu/homebridge](https://hub.docker.com/r/oznu/homebridge) \
GitHub: [oznu/homebridge](https://github.com/oznu/docker-homebridge)

### [Airconnect]()
Turning Chromecast into Airplay targets. \
DockerHub: [1activegeek/airconnect](https://hub.docker.com/r/1activegeek/airconnect) \
GitHub: [1activegeek/docker-airconnect](https://github.com/1activegeek/docker-airconnect)

## security-apps
### [Nginx-Proxy-Manager](https://nginxproxymanager.com)
Proxy server that expose your services easily and securely. \
DockerHub: [jc21/nginx-proxy-manager](https://hub.docker.com/r/jc21/nginx-proxy-manager) \
GitHub: [jc21/nginx-proxy-manager](https://github.com/jc21/nginx-proxy-manager)

### [Vaultwarden](https://bitwarden.com/)
Offers the easiest and safest way for teams and individuals to store and share sensitive data from any device. \
DockerHub: [vvaultwarden/server](https://hub.docker.com/r/vaultwarden/server) \
GitHub: [bitwarden/server](https://github.com/bitwarden/server)

### [adGuardHome](https://adguard.com/en/welcome.html)
AdGuardHome is a network-wide software for blocking ads and tracking. After you set it up, it'll cover all your home devices, and you won't need any client-side software for that. \
DockerHub: [adguard/adguardhome](https://hub.docker.com/r/adguard/adguardhome) \
GitHub: [AdguardTeam/AdGuardHome](https://github.com/AdguardTeam/AdGuardHome/wiki/Docker)

### [Pi-hole](https://pi-hole.net)
Network-wide Ad Blocking. \
DockerHub: [pihole/pihole](https://hub.docker.com/r/pihole/pihole) \
GitHub: [pi-hole/pi-hole](https://github.com/pi-hole/docker-pi-hole/#running-pi-hole-docker)

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

## monitoring-apps
### [Scrutiny]()
WebUI for smartd S.M.A.R.T monitoring. Scrutiny is a Hard Drive Health Dashboard & Monitoring solution, merging manufacturer provided S.M.A.R.T metrics with real-world failure rates from Backblaze. \
DockerHub:  [linuxserver/scrutiny](https://hub.docker.com/r/linuxserver/scrutiny) \
GitHub: [AnalogJ/scrutiny](https://github.com/AnalogJ/scrutiny#docker)

### [Uptime-kuma](https://demo.uptime.kuma.pet:27000)
Uptime Kuma is an easy-to-use self-hosted monitoring tool. \
DockerHub: [louislam/uptime-kuma](https://hub.docker.com/r/louislam/uptime-kuma) \
GitHub: [louislam/uptime-kuma](https://github.com/AnalogJ/scrutiny#docker)

### [Speedtest](https://speedtest.henrywhitaker.com)
This program runs a speedtest check every hour and graphs the results. \
DockerHub: [henrywhitaker3/speedtest-tracker](https://hub.docker.com/r/henrywhitaker3/speedtest-tracker) \
GitHub: [henrywhitaker3/speedtest-tracker](https://github.com/henrywhitaker3/Speedtest-Tracker)

## additional-apps
### [Heimdall](https://heimdall.site)
Is a way to organise all those links to your most used web sites and web applications in a simple way. Simplicity is the key to Heimdall. Why not use it as your browser start page? \
DockerHub: [linuxserver/heimdall](https://hub.docker.com/r/linuxserver/heimdall) \
GitHub:[linuxserver/Heimdall](https://github.com/linuxserver/Heimdall)

### Owntone
(iTunes) is a media server with support for AirPlay devices, Apple Remote (and compatibles), Chromecast, MPD and internet radio. \
DockerHub: [owntone/forked-daapd](https://github.com/owntone/forked-daapd) \
GitHub: [linuxserver/daapd](https://hub.docker.com/r/linuxserver/daapd)

### Watchtower
With watchtower you can update the running version of your containerized app simply by pushing a new image to the Docker Hub or your own image registry. Watchtower will pull down your new image, gracefully shut down your existing container and restart it with the same options that were used when it was deployed initially. \

DockerHub: [containrrr/watchtower](https://hub.docker.com/r/containrrr/watchtower) \
GitHub: [containrrr/watchtower](https://github.com/containrrr/watchtower)

### [Transmission](https://transmissionbt.com)
A Fast, Easy and Free Bittorrent Client For macOS, Windows and Linux. \
GitHub: [linuxserver/docker-transmission](https://github.com/linuxserver/docker-transmission)

to be updated:
> TimeMachine, Teedy, Readarr, Prism, Photostructure, Nextcloud, Elkarbackup, Duckdns

## Info
Because all the services are setup with `docker-compose` they can all reach each other by their Docker Compose service name. So for example when connecting Sonarr with Jacket or qBittorrent, then Jackett would be available on `http://jackett/api....`, which makes everything a lot easier.

### Edit the .env file
All configuration to this setup, I've put in the `.env` file, so all you have to do is go through it and edit it to fit your needs.
