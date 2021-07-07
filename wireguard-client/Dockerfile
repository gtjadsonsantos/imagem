FROM alpine:latest

RUN apk --no-cache add wireguard-tools iptables ip6tables inotify-tools

COPY run .

RUN \
    chmod +x run

VOLUME /etc/wireguard

CMD ["/run"]