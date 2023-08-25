# Docker-Angular-Demo
Demo dockerize Angular app

## BUILD A IMAGE

Go to directory ```Docker-Angular-Demo/angular-hello-world/```

```
# build web-app in production using nginx server
docker build -t angular-hello-world:prod .

# build web-app in dev without using nginx server
docker build -t angular-hello-world:dev -f Dockerfile.dev .
```

## RUN A CONTAINER FROM IMAGE

```
# run a container from image with prod tag and export at port 80
docker run -p 80:80  angular-hello-world:prod

# run a container from image with dev tag and export at port 4200
docker run -p 4200:4200  angular-hello-world:dev
```

