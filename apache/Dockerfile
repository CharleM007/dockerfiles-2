FROM amazonlinux:2
MAINTAINER Tung Nguyen <tongueroo@gmail.com>

# Common tools
RUN yum update -y && \
  yum install -y \
    findutils \
    jq \
    less \
    net-tools \
    procps \
    tree \
    unzip \
    vim \
    tar \
    wget && \
  yum clean all && \
  rm -rf /var/cache/yum

COPY container/install-apache.sh /tmp/install-apache.sh
RUN chmod a+x /tmp/install-apache.sh
RUN /tmp/install-apache.sh

EXPOSE 80

CMD ["/usr/sbin/httpd", "-DFOREGROUND"]
# /usr/sbin/httpd -DFOREGROUND
