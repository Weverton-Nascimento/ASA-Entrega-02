
FROM ubuntu:latest 

RUN apt update -y
RUN apt upgrade -y
RUN apt install bind9 dnsutils -y

COPY named.conf.local /etc/bind
COPY db.asa.br /etc/bind

CMD ["/usr/sbin/named", "-g", "-c", "/etc/bind/named.conf", "-u", "bind"]
