#
# Dockerfile for collectd
#

FROM alpine
MAINTAINER kev <noreply@datageek.info>

RUN apk add -U collectd collectd-dev \
    && rm -rf /var/cache/apk/*

COPY ./collectd /etc/collectd
VOLUME /etc/collectd

CMD ["collectd", "-f"]
