FROM golang:1.23rc2 AS builder
COPY . src/
RUN cd src && ls && GOPROXY=direct go build -o ../bin/worker ./cmd/worker/

ENTRYPOINT [ "/go/bin/worker" ]