FROM golang

WORKDIR /usr/src/app

COPY . .

RUN exec bash

RUN go build

RUN go test ./...

CMD ["./server"]
