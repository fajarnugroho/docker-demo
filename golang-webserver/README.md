# Golang-WebServer

## Docker Multistage Build

Simple Webserver Golang.

## How to run

1. build image

```sh
$ docker build -t go-webserver .
```

2. run image

```
$ docker run -d -p 3000:3000 go-webserver
```

3. open localhost:3000 in browser
