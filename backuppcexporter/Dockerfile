FROM ubuntu:focal
MAINTAINER Álvaro Castellano Vela <alvaro.castellano.vela@gmail.com>

COPY backuppcexporter/backuppc_exporter /usr/local/bin/backuppc_exporter

RUN useradd -ms /bin/bash backuppc
RUN usermod -a -G users backuppc
RUN chmod 755 /usr/local/bin/backuppc_exporter

USER backuppc

EXPOSE 8080

STOPSIGNAL SIGTERM

CMD ["/usr/local/bin/backuppc_exporter"]
