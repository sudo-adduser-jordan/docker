# docker server

A simple self hosted solution for developers. 


```sh

# download
git https://github.com/sudo-adduser-jordan/docker; cd docker 

# execute 
docker compose up -d

# registir git runner
docker exec -it git-runner forgejo-runner register # https://git:3000

# backup
# sudo cp /var/lib/docker/volumes /path/to/your/backups

```

```sh
# source <(curl https://dblocks.net/server)
```

# programs
```sh

network # network.exampledomain.com
piehole # adblock.exampledomain.com
portainer # docker.exampledomain.com
forgejo # git.exampledomain.com
komodo # build.exampledomain.com
openspeedtest # speed.example.domain.com

```


# commands
```sh
# local ssl generate
openssl req -x509 -newkey rsa:4096 -keyout key.pem -out cert.pem -sha256 -days 365 -nodes # not reccommended, use caddy certificate instead

# download local ssl

# setup local ssl 
git config http.sslVerify false # not reccommended
git config --global http.sslCAInfo /root/git-dblocks-net.pem 
# git config --system http.sslCAInfo /root/git-dblocks-net.pem 

# registir runner 
docker exec -it git-runner forgejo-runner register # https://git:3000

```

# resources
```sh

# programs
https://komo.do/
https://pi-hole.net/
https://forgejo.org/
https://www.docker.com/
https://www.portainer.io/
https://openspeedtest.com/
https://atlasdemo.vnerd.nl/
https://github.com/karam-ajaj/atlas

# docs
https://forgejo.org/docs/v14.0/admin/actions/runner-installation/#oci-image-installation
https://emasblog.dev/posts/2025/11/forgejo-runners-container-setup/

```

# todo
```sh

- vpn

```


