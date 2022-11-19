# trukos-caprover

https://caprover.com/docs/get-started.html

# Install
```
docker run -p 80:80 -p 443:443 -p 3000:3000 -v /var/run/docker.sock:/var/run/docker.sock -v /captain:/captain caprover/caprover
```


# Uninstall
```
$ docker stop $(docker ps -a -q)
$ docker rm $(docker ps -a -q)
```
