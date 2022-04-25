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

Requests get routed according to thw weights of the route. 80% to the service1 and 20% to the service2.

```
for i in {1..10}; do curl -si localhost:8080/version; done
```
