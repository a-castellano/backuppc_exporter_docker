FROM ubuntu:focal
MAINTAINER Álvaro Castellano Vela <alvaro.castellano.vela@gmail.com>

COPY backuppc_exporter /usr/local/bin/backuppc_exporter

RUN chmod 755 /usr/local/bin/backuppc_exporter

EXPOSE 8080

STOPSIGNAL SIGTERM

CMD ["/usr/local/bin/backuppc_exporter"]
