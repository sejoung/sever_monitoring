# sever_monitoring

```
docker run -d --gpus all --cap-add SYS_ADMIN --restart unless-stopped -p 9400:9400 nvidia/dcgm-exporter:4.1.1-4.0.4-ubuntu22.04
```

```
docker run -d --restart unless-stopped -p 9100:9100 prom/node-exporter:latest
```

```
docker pull nvidia/dcgm-exporter:4.1.1-4.0.4-ubuntu22.04

docker pull prom/node-exporter:latest
```
