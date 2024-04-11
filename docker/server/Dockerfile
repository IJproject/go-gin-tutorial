FROM golang:latest
WORKDIR /app
COPY ./server .
RUN go mod download
EXPOSE 8080
CMD ["go", "run", "main.go"]