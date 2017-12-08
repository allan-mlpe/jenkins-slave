# jenkins-slave

<h3>Instructions</h3>

- Building locally, from whitin the Dockerfile directory:
```
docker build -t jenkins-slave:$TAG .
```

- Preventing caching on build:
```
docker build --no-cache -t jenkins-slave:$TAG
```
