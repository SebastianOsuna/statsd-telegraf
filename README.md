## See https://hub.docker.com/_/telegraf/

Telegraf configured with UDP Statsd input and InfluxDB output
---

Added configurations:

### INFLUXDB_HOST

Defaults to `localhost`

### INFLUXDB_PORT

Defaults to `8086`

### INFLUXDB_DATABASE

Defaults to `db0`


```cli
docker run -d --name telegraf -e INFLUXDB_HOST=influxdb.example.com -e INFLUXDB_PORT=8086 -e INFLUXDB_DATABASE=db0 -p 8125:8125/udp sebastianosuna/statsd-telegraf:latest
```
