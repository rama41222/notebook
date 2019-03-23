### Accessing host from docker container

If you have a docker-compose.yml you can add the following to access host.

###### Using docker-compose

`network_mode: "host"`

Sample **docker-compose.yml**

```
version: '3'
services:
  webapp:
    image: myservice
    build: .
    ports:
      - "3000:3000"
    env_file:
      - .env
    network_mode: "host"
```

###### Using docker run
```
docker run -it --net=host  
docker run -it --network=host
```

### Accessing host from docker container in MAC

You can now access the mad host running services within a docker container using the following address.

- Docker for Mac v17.12 and Above
`docker.for.mac.localhost`

- Docker for Mac  v17.06 to v 17.11
`docker.for.mac.host.internal`

[Release Note](https://docs.docker.com/docker-for-mac/release-notes/#docker-community-edition-17060-ce-mac18-2017-06-28-stable)
 
