FROM golang:1.10-alpine3.8  AS builder
RUN apk add git gcc libpcap libpcap-dev libbsd-dev
RUN go get github.com/hsiafan/httpdump





FROM alpine:3.8
RUN yum install -y libpcap-dev
COPY --from=builder /go/src/bin/httpdump /usr/bin/httpdump






