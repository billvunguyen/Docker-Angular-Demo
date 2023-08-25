# Docker-Angular-Demo
Demo dockerize Angular app

## BUILD A IMAGE

```
docker build -t angular-hello-world:prod . # build web-app in production using nginx server

docker build -t angular-hello-world:dev -f Dockerfile.dev . # build web-app in dev without using nginx server
```

## RUN A CONTAINER FROM IMAGE

```
docker run -p 80:80  angular-hello-world:prod # run a container from image with prod tag and export at port 80

docker run -p 4200:4200  angular-hello-world:dev # run a container from image with dev tag and export at port 4200
```

