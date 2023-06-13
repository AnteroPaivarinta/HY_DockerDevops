FROM golang:1.16-alpine
WORKDIR /
COPY example-backend .
RUN go build

EXPOSE 8000
ENTRYPOINT ["./server"]
