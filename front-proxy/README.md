## Running this code 

#### To start the compose stack 
```
docker-compose up -d --build
```

#### To delete the compose stack 
```
docker-compose down
```

## Goal

Basic round robin load balancing of services by front proxy.


```
curl -si localhost:8080/service/1
curl -si localhost:8080/service/2
```