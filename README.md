# docker server

A simple self hosted solution for developers. 


```sh
# download
git https://github.com/sudo-adduser-jordan/docker; cd docker 

# execute 
docker compose up -d

# registir git runner
# docker exec -it git-runner forgejo-runner register
docker exec -it git-runner \
  forgejo-runner register \
  --instance https://git.dblocks.net \
  --token l9spxBt8PuCNhORUpEWpAXZpvoJNzT6zdrgmNL9R \
  --name "git-runner" \
  --no-interactive


# configure git to use local ssl
git config --global http.sslCAInfo /docker/certificates/local/git.dblocks.net/git.dblocks.net.crt 

# backup
cp /var/lib/docker/volumes /path/to/your/backups

```

or

```sh
source <(curl https://dblocks.net/install)
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


