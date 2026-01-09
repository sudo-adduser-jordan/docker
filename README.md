# docker

https://hub.docker.com/

git https://github.com/sudo-adduser-jordan/docker
curl https://raw.githubusercontent.com/louislam/dockge/master/compose.yaml --output compose.yaml

docker compose up -d
docker container prune

sudo docker ps -q | xargs -r sudo docker stop
sudo docker ps -a -q | xargs -r sudo docker rm -f
sudo docker images -q | xargs -r sudo docker rmi -f
sudo docker volume prune -f
sudo docker network prune -f
sudo docker system prune -a --volumes -f


docker run -d --restart=always -p 3001:3001 -v uptime-kuma:/app/data --name uptime-kuma louislam/uptime-kuma:2




sudo docker ps
 sudo docker inspect --format '{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' 7090e8a3c57a


docker container prune -f


docker ps -q | xargs -r docker kill
sudo docker kill containername



openssl req -newkey rsa:2048 -new -nodes -x509 -days 3650 -keyout selfsigned.pem -out selfsigned.crt

sudo docker exec -it headscale headscale apikeys create --expiration 90d

sudo docker exec -it headscale headscale users create user1
sudo docker exec -it headscale headscale pre-authkeys create --user user1


https://github.com/karam-ajaj/atlas
https://github.com/henrygd/beszel