# Quagga BGP

FROM alpine:latest

RUN apk update
RUN apk add --no-cache bind-tools
RUN apk add nano 
CMD ["named", "-c", "/etc/bind/named.conf", "-g", "-u", "named"]
