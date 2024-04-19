# resumedocker
# Installing
```
apt update
```
```
apt install docker.io
```
# Finding process
ALL process
```
docker ps
```
RUNNING process
```
docker ps -a
```

# commiting docker [eg](https://phoenixnap.com/kb/how-to-commit-changes-to-docker-image)
Make docker ps,  to commit th
```
docker ps -a
```
do docker commit [container id] [new_image] </br>
or docker commit [container id] [image_name]:[tag]
```
docker commit  cc43 new_image
```
```
docker image  ls
```
# Create container by image on local (before commiting)
```
docker run -tid new_image --name new_image_container sh
```

# Executing sh
docker exec -ti name new_image_container  /bin/sh


# SAVING BY TAR AND LOADING IMAGES [eg](https://pspdfkit.com/blog/2019/docker-import-export-vs-load-save/)
```
docker save new_image > name_image.tar.gz
```
```
docker load < name_image.tar.gz
```

# PUSH AND PULL
[eg](https://www.geeksforgeeks.org/docker-commit/)

# VIDEO 1 : 
## Upload OS nginx latestover docker
```
docker run -tid -p 8080:80 --name web nginx:latest
```

## For inspection
```
docker inspect 
```
or
```
docker inspect | grep IPAddress
```
# VIDEO 2 : Persistance
```
docker start web 
```

```
docker exec -tid web sh
```
ON WEB CONTAINERS
```
apt update
```
```
apt install vim
```
```
vim /us/share/nginx/html/index.html
```
