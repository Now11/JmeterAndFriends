FROM grafana/grafana:6.4.1

USER root

RUN apk update \
    && rm -rf /var/lib/apk/lists/*

WORKDIR /etc/grafana

COPY datasources ./datasources

WORKDIR /app
COPY entrypoint.sh ./
RUN ["chmod", "u+x", "entrypoint.sh"]
ENTRYPOINT ["/app/entrypoint.sh"]
