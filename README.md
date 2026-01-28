# docker server

A simple self hosted solution for developers. 


```sh
# download
git https://github.com/sudo-adduser-jordan/docker; cd docker 

# execute 
docker compose up -d

# registir git runner
docker exec -it git-runner \
  forgejo-runner register \
  --instance http://10.0.0.5:1026 \
  --token hOmDhkqMMwVxGPtNXEh8Kx3NqB4gvRwUvKV6TlOC \
  --name "git-runner" \
  --no-interactive

# backup
cp /var/lib/docker/volumes /path/to/your/backups

# configure client to use local ssl
cp ./etc/hosts /etc/hosts 
cp ./etc/ssl/certs/ca-certificates.crt /etc/ssl/certs/ca-certificates.crt 
update-ca-certificates

# sudo cp caddy-local-authority--ecc-intermediate.pem /etc/pki/ca-trust/source/anchors/
# sudo update-ca-trust extract


# piehole with filter the host device
# to have pihole filter your entire network you must point your router to your hosts internal ip in the router settings
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
- regisitir runner automagically
```


