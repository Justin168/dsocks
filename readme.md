# DSOCKS
Docker hosted shadowsocks server

## Configuration
Edit **conf/config.json**
```json
{
    "server":"0.0.0.0",
    "server_port":8388,
    "local_address": "127.0.0.1",
    "local_port":1080,
    "password":"123456",
    "timeout":300,
    "method":"aes-256-cfb",
    "fast_open": false
}
```
The configuration file is mounted as a volume, you may edit and restart server without rebuilding.

## Start Server
```shell
docker-compose up -d
```

## Restart Server
```shell
docker-compose restart
```

## Stop Server
```shell
docker-compose stop
```