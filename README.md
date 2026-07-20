# docker

[![Repo Size](https://img.shields.io/github/repo-size/sudo-adduser-jordan/docker)](https://github.com/sudo-adduser-jordan/docker)
[![Last Commit](https://img.shields.io/github/last-commit/sudo-adduser-jordan/docker)](https://github.com/sudo-adduser-jordan/docker)
[![Docker](https://img.shields.io/badge/Docker-Compose-2496ED?logo=docker&logoColor=white)](https://docs.docker.com/compose/)

A simple self hosted solution for developers.

```sh
source <(curl https://github.com/sudo-adduser-jordan/docker/install)
```

```sh
git clone https://github.com/sudo-adduser-jordan/docker 
cd docker 
cp .example.env .env
sudo docker compose up -d
sudo resolvectl dns eth0 127.0.0.1 # use pihole for host dns (non-persistent, re-run after reboot)

# sudo resolvectl dns enp3s0 127.0.0.1 # use pihole for host dns (non-persistent, re-run after reboot)
# sudo resolvectl domain enp3s0 "~."
# sudo resolvectl dns pvpn0 127.0.0.1
# sudo resolvectl domain pvpn0 "~."
```


```sh
git clone https://github.com/sudo-adduser-jordan/docker 
cd docker 
cp .example.env .env
sudo docker compose up -d
sudo resolvectl dns eth0 127.0.0.1 # use pihole for host dns (non-persistent, re-run after reboot)
```

```sh
piehole # adblock.exampledomain.com
forgejo # git.exampledomain.com
postgres # db.dblocks.net
```

## resources
```sh
# programs
https://pi-hole.net/
https://forgejo.org/
https://www.docker.com/
https://www.postgresql.org/
https://www.pgadmin.org/

# docs
https://forgejo.org/docs/v14.0/admin/actions/runner-installation/#oci-image-installation
https://emasblog.dev/posts/2025/11/forgejo-runners-container-setup/

```
