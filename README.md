# docker server
```sh
git https://github.com/sudo-adduser-jordan/docker
docker compose up -d
```

# programs
```sh
beszel # metrics.exampledomain.com
dockge # docker.exampledomain.com
forgejo # git.exampledomain.com
kuma # uptime.exampledomain.com

```

# commands
```sh
# generate nginx certifications
mkdir -p certs
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout ./certs/nginx.key -out ./certs/nginx.crt
```

# resources
```sh
https://hub.docker.com/
https://github.com/karam-ajaj/atlas
https://github.com/henrygd/beszel

```


# todo
```sh

- web stack
- adgaurd
- vpn
- paas
- 


```