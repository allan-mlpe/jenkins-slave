# jenkins-slave

# Suported tags and respective Dockerfile links
- `latest`: [full/Dockerfile](https://github.com/allan-mlpe/jenkins-slave/blob/master/full/Dockerfile)
- `angular`: [angular/Dockerfile](https://github.com/allan-mlpe/jenkins-slave/blob/master/angular/Dockerfile)
- `maven`: [maven/Dockerfile](https://github.com/allan-mlpe/jenkins-slave/blob/master/maven/Dockerfile) 
- `sbt`: [sbt/Dockerfile](https://github.com/allan-mlpe/jenkins-slave/blob/master/sbt/Dockerfile)

# Instructions

- Running a slave:

```
docker run -d allanmlpe/jenkins-slave:latest
```

- Building locally, from whitin the Dockerfile directory:
```
docker build -t jenkins-slave:$TAG .
```

- Preventing caching on build:
```
docker build --no-cache -t jenkins-slave:$TAG .
```

- Build imagem with docker-compose (add `--no-cache` option to prevent caching on build):
```
docker-compose build [--no-cache]
```

- Running a slave with docker-compose:
```
docker-compose up -d
```

# Docker Hub

- [allanmlpe/jenkins-slave](https://hub.docker.com/r/allanmlpe/jenkins-slave/)