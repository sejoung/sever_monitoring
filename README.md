# prometheus

## 서버 실행 방법

```
docker compose up -d
```

### import

dahsboard.json 파일을 import 하면 됩니다.

datasource uid는 바꿔야 됩니다.

아래는 대쉬보드 id 참고용
```
12486

12239
```

## 클라이언트 설치

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
