FROM centos:centos7  AS builder
RUN yum install -y git gcc libpcap libpcap-devel
RUN go get github.com/hsiafan/httpdump





FROM centos:centos7
RUN yum install -y libpcap-dev
COPY --from=builder /go/src/bin/httpdump /usr/bin/httpdump






