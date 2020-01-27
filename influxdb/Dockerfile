FROM influxdb:1.7.9-alpine

WORKDIR /app
COPY entrypoint.sh ./

RUN ["chmod", "+x", "entrypoint.sh"]
ENTRYPOINT ["/app/entrypoint.sh"]
