## nginx images

### FROM

- nginx:1.13.0 
- https://github.com/nginxinc/docker-nginx/blob/53da9a295dfa6c666630a72d9c03dfbd1d2eb37d/mainline/stretch/Dockerfile

### 构建地址

- https://cr.console.aliyun.com/repository/cn-beijing/meow/nginx/build

### 镜像名称

- registry.cn-beijing.aliyuncs.com/meow/nginx:1.13.0

### 使用方法

```bash

docker run -d -p 8080:80  registry.cn-beijing.aliyuncs.com/meow/nginx:1.13.0

# nginx.conf

cat /etc/nginx/nginx.conf

cat /etc/nginx/conf.d/default.conf 
server {
    listen       80;
    server_name  localhost;

    #charset koi8-r;
    #access_log  /var/log/nginx/log/host.access.log  main;

    location / {
        root   /usr/share/nginx/html;
        index  index.html index.htm;
    }


```
