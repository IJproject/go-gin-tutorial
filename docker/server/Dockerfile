FROM golang:latest
WORKDIR /app
COPY ./server .
RUN go mod download
RUN go get -u github.com/cosmtrek/air && \
    go build -o /go/bin/air github.com/cosmtrek/air
EXPOSE 8080
CMD ["air", "-c", ".air.toml"]