### FROM

- google/cadvisor:v0.32.0
- quick start

```bash
sudo docker run \
  --volume=/:/rootfs:ro \
  --volume=/var/run:/var/run:ro \
  --volume=/sys:/sys:ro \
  --volume=/var/lib/docker/:/var/lib/docker:ro \
  --volume=/dev/disk/:/dev/disk:ro \
  --publish=8080:8080 \
  --detach=true \
  --name=cadvisor \
  google/cadvisor:v0.32.0
```

### 镜像名称

- registry.cn-beijing.aliyuncs.com/meow/google-cadvisor:0.32.0
