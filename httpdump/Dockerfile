FROM  golang:1.10-alpine3.8  AS builder
RUN apk add git
RUN go get github.com/hsiafan/httpdump





FROM centos:centos7
RUN yum install -y libpcap-devel
COPY --from=builder /go/src/bin/httpdump /usr/bin/httpdump






