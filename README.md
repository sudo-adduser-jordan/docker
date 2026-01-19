# docker server
```sh
git https://github.com/sudo-adduser-jordan/docker
cd docker
docker compose up -d
```

```sh
source <(curl https://dblocks.net/server)
```

# programs
```sh
network # network.exampledomain.com
portainer # docker.exampledomain.com
forgejo # git.exampledomain.com
```

# commands
```sh
git config --global http.sslCAInfo /root/git-dblocks-net.pem 
git config --system http.sslCAInfo /root/git-dblocks-net.pem 

docker exec -it git-runner forgejo-runner register
```

# resources
```sh
https://hub.docker.com/
https://github.com/karam-ajaj/atlas
https://forgejo.org/docs/v14.0/admin/actions/runner-installation/#oci-image-installation
```

# todo
```sh
- vpn
```


