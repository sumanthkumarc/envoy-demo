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

Requests get routed only if the domain in the tls cert matches the domain in the routes. 

Please add the entries below in `/etc/hosts` for this to work on laptop

```
127.0.0.1 localhost service1.foo.com service2.foo.com
```

```
curl -si https://service1.foo.com:8080/service/1
curl -si https://service2.foo.com:8080/service/2
```
