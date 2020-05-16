# Simple Dockerfile build

## Credit
[miguelgrinberg/flask-examples](https://github.com/miguelgrinberg/flask-examples)


## How to run

1. build image

```sh
$ docker build -t helloworld .
```

2. run image

```sh
$ docker run -p 5000:5000 helloworld
```

3. open localhost:5000 in browser
