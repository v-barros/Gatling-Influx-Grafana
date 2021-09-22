FROM influxdb:1.8-alpine

WORKDIR /app
COPY entrypoint.sh ./
RUN chmod u+x entrypoint.sh
COPY influxdb.conf /etc/influxdb/influxdb.conf
RUN echo ${INFLUX_DB}
ENTRYPOINT ["/app/entrypoint.sh"]