# MQTT LB Nginx

## Useage

```bash
docker compose up -d
```

Open <http://localhost:18083> to visit EMQX Dashboard.

## Test

EMQX MQTT TCP

```bash
$ mqttx sub --config ./mqttx_cli_emqx_tcp.json

[2023-8-22] [22:26:21] › …  Connecting using configuration file, host: localhost, port: 1883, topic: t/1
[2023-8-22] [22:26:21] › ✔  Connected
[2023-8-22] [22:26:21] › …  Subscribing to t/1...
[2023-8-22] [22:26:21] › ✔  Subscribed to t/1
```

EMQX MQTT TLS

```bash
$ mqttx sub --config ./mqttx_cli_emqx_tls.json

[2023-8-22] [22:26:54] › …  Connecting using configuration file, host: undefined, port: 8883, topic: t/1
[2023-8-22] [22:26:54] › ✔  Connected
[2023-8-22] [22:26:54] › …  Subscribing to t/1...
[2023-8-22] [22:26:54] › ✔  Subscribed to t/1
```