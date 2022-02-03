# NGINX setup

In root directory of project:
```
docker build -t desired-name .
```

then:

```
docker run --name nginx -d -p 8080:80 desired-name
```

navigate to http://localhost:8080 or http://host-ip:8080


## Open a shell in the running container

If you want to look around the container, get the running docker containers' ID: 

```
docker container ls
```

then: 

```
docker exec -it CONTAINER-ID bin/bash
```

type exit to exit
