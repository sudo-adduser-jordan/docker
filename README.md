# docker server
```sh
git https://github.com/sudo-adduser-jordan/docker
cd docker
mkdir -p certs
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout ./certs/nginx.key -out ./certs/nginx.crt
docker compose up -d
```

```sh
source <(curl https://github.com/sudo-adduser-jordan/docker/install)
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
mkdir -p certs
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout ./certs/nginx.key -out ./certs/nginx.crt
```

# resources
```sh
https://hub.docker.com/
https://github.com/karam-ajaj/atlas

```

# todo
```sh
- vpn
- adgaurd
- cd
```