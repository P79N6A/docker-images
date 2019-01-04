### Description
jenkins master install

### Usage
Use it with docker-compose    

```
#部署

docker  run -d -v /home/workspace/jenkins-master:/var/jenkins_home -p 8080:8080 registry.cn-beijing.aliyuncs.com/meow/jenkins-master:2.19.2

#登录
http://localhost:8080/    #docker logs  ContainerID 查看默认密码；跳过推荐插件安装

```
