FROM golang:1.13 AS build-env

WORKDIR /build
COPY go.mod go.sum ./
RUN go mod download


COPY . /build

RUN go build -ldflags="-w -s" -o go-webserver .

FROM debian:stretch

WORKDIR /app
COPY --from=build-env /build/go-webserver /app/webserver

CMD [ "/app/webserver" ]
