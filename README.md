# IoT Data Collector

- Docker compose that connects an MQTT Broker, Telegraph for parsing, InfluxDB and Grafana
- For changes in connections create a new telegraf container with its own config
- Recommended Tools
    - MQTT Explorer 
    - Time Series Admin
- Usage: `docker-compose up -d`
- local MQTT:
    -bobm/letmein
- Grafana:
 - bobgra/letmein


## Known-issues

-[x] Influx VB Version is 1.8. which is ok for now
-[] Data Model in the influx is not nice (find nice example for good practise?)  https://docs.influxdata.com/influxdb/cloud/reference/key-concepts/data-elements/
-[x] No secure encryption
-[x] Undefined data storage location and no backup (docker volumes) search for persistancy (now bound to folder)
-[x] chronograph?




- [] change Tailscale admin


## Setting up
for chronograf change the URL (default: http://influxdb:8086) to your actual IP 
