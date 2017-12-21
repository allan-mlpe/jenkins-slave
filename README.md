# jenkins-slave

# Suported tags and respective Dockerfile links
- `latest`: [full/Dockerfile](https://github.com/allan-mlpe/jenkins-slave/blob/master/full/Dockerfile)
- `angular`: [angular/Dockerfile](https://github.com/allan-mlpe/jenkins-slave/blob/master/angular/Dockerfile)
- `maven`: [maven/Dockerfile](https://github.com/allan-mlpe/jenkins-slave/blob/master/maven/Dockerfile) 
- `sbt`: [sbt/Dockerfile](https://github.com/allan-mlpe/jenkins-slave/blob/master/sbt/Dockerfile)

# Instructions

- Building locally, from whitin the Dockerfile directory:
```
docker build -t jenkins-slave:$TAG .
```

- Preventing caching on build:
```
docker build --no-cache -t jenkins-slave:$TAG
```

# Docker Hub

- [allanmlpe/jenkins-slave](https://hub.docker.com/r/allanmlpe/jenkins-slave/)