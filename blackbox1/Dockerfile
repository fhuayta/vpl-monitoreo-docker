FROM        quay.io/prometheus/busybox:latest
MAINTAINER  The Prometheus Authors <prometheus-developers@googlegroups.com>

COPY blackbox_exporter  /bin/blackbox_exporter
COPY blackbox.yml       /etc/blackbox/blackbox.yml

EXPOSE      9115
ENTRYPOINT  [ "/bin/blackbox_exporter" ]
CMD         [ "--config.file=/etc/blackbox/blackbox.yml" ]