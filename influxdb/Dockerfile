FROM influxdb:1.7.9-alpine

WORKDIR /root

RUN apt-get -y update

# Configure InfluxDB
COPY influxdb/influxdb.conf /etc/influxdb/influxdb.conf
COPY influxdb/init.sh /etc/init.d/influxdb

RUN chmod 0755 /etc/init.d/influxdb

RUN ["chmod", "+x", "entrypoint.sh"]

