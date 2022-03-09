# MQTT / Grafana

A docker compose stack with:

- An MQTT broker (eclipse mosquitto)
- InfluxDB
- telegraf server agent to connect the MQTT broker to the database
- Grafana for graphs

Everything (mosquitto, influxdb and grafana) have the same user/password:

- user: `admin`
- password: `password`

Grafana is already configured with the InfluxDB datasource.

Note: This stack doesn't use influxdb verison 2, I had issues making grafana
talk to the database.

Warning: the security of this stack is not great, use at your own risk.
