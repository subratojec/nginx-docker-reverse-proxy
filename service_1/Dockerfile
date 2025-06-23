FROM golang:1.24.2-alpine

RUN apk update && apk add --no-cache curl 

WORKDIR /app

COPY . /app

RUN go build -o main . 

EXPOSE 8001

CMD ["./main"]