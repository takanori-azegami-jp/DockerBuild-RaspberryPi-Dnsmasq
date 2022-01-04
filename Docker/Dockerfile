FROM resin/rpi-raspbian

RUN apt-get update
RUN apt-get -q -y install dnsmasq

VOLUME /etc/hosts

CMD dnsmasq -k

EXPOSE 53 53/udp