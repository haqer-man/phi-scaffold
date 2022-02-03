# NGINX setup

In root directory of project:
```
docker build -t custom-name .
```

then:

```
docker run --name nginx -d -p 8080:80 custom-name
```

navigate to http://localhost:8080 or http://host-ip:8080


## Open a shell in the running container

If you want to look around the container, get the running docker containers' ID: 

```
docker ps
```

then: 

```
docker exec -it CONTAINER-ID bin/bash
```

type exit to exit
