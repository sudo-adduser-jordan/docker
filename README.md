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
nginx # nginx.exampledomain.com
network # network.exampledomain.com
portainer # docker.exampledomain.com
forgejo # git.exampledomain.com
```

# commands
```sh
echo | openssl s_client -servername server -connect 10.0.0.5:3000 | openssl x509 -outform PEM > git-dblock-net.pem
git config --global http.sslCAInfo ~/git-dblocks-net.pem 

```

# resources
```sh
https://hub.docker.com/
https://github.com/karam-ajaj/atlas

```

# todo
```sh
- vpn
```


