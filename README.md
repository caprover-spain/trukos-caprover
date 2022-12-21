# Tips CapRover

https://caprover.com/docs/get-started.html

# Actualizamos el sistema
```
apt-get update && apt-get upgrade -y
```

# Install CapRover
```
ufw allow 80,443,3000,996,7946,4789,2377/tcp; ufw allow 7946,4789,2377/udp;
apt  install docker.io
docker run -p 80:80 -p 443:443 -p 3000:3000 -v /var/run/docker.sock:/var/run/docker.sock -v /captain:/captain caprover/caprover
npm i -g caprover
caprover serversetup
```


# Uninstall CapRover
```
$ docker stop $(docker ps -a -q)
$ docker rm $(docker ps -a -q)

$ docker service rm $(docker service ls -q)
$ docker swarm leave --force
```

```
$ docker build -t mfalconsoft/caprover-nodejs .
$ docker push mfalconsoft/caprover-nodejs
$ docker images
$ docker run -d -p 3000:3000 mfalconsoft/caprover-nodejs
```

# Listar volumenes
```
docker volume ls
/var/lib/docker/volumes/captain--odoo13-config/_data
```
