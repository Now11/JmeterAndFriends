FROM grafana/grafana:6.4.1

WORKDIR /root


# Configure Grafana
COPY datasources ./datasources
COPY grafana/grafana.ini /etc/grafana/grafana.ini

RUN ["chmod", "+x", "entrypoint.sh"]
