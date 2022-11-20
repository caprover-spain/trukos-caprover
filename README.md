# Tips CapRover

https://caprover.com/docs/get-started.html
 
# Install CapRover
```
apt  install docker.io
docker run -p 80:80 -p 443:443 -p 3000:3000 -v /var/run/docker.sock:/var/run/docker.sock -v /captain:/captain caprover/caprover
npm i -g caprover
caprover serversetup
```


# Uninstall CapRover
```
$ docker stop $(docker ps -a -q)
$ docker rm $(docker ps -a -q)
```

```
$ docker build -t mfalconsoft/caprover-nodejs .
$ docker push mfalconsoft/caprover-nodejs
$ docker images
$ docker run -d -p 3000:3000 mfalconsoft/caprover-nodejs
```
