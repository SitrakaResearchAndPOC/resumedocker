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
docker ps -a
```
RUNNING process
```
docker ps -a
```

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
