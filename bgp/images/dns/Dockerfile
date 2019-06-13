FROM alpine:latest
RUN apk add --no-cache bind-tools
RUN apk --update add bind
RUN apk add nano 

COPY bind /etc/bind

RUN /bin/ash -c "chmod -R 777 /etc/bind"
RUN /bin/ash -c "mkdir /var/cache/bind"
RUN /bin/ash -c "chmod -R 777 /var/cache/bind"

EXPOSE 53/udp 53/tcp 10000/tcp
CMD ["named", "-c", "/etc/bind/named.conf", "-g", "-u", "named"]


