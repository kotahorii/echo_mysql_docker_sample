FROM golang:1.17.3-alpine3.14
RUN mkdir /go/src/api
WORKDIR /go/src/api
COPY ./api /go/src/api/
VOLUME /go/src/api
RUN go mod download
EXPOSE 8080
CMD "go" "run" "main.go"