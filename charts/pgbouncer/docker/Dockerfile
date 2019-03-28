FROM ubuntu:18.10
RUN apt-get update && apt install -y pgbouncer postgresql-client-10
RUN useradd pgbouncer -b '/' -m
USER pgbouncer
COPY run.sh /run.sh
COPY do_probe.sh /do_probe.sh
ENTRYPOINT /run.sh
