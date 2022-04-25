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

Requests get rate limited after more than 2 requests in span of 5s.

```
for i in {1..10}; do curl -si localhost:8080/service/1; done
```
