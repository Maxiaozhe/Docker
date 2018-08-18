# Docker 笔记
Docker 常用命令
## 创建容器


## 管理容器
### 容器列表
```
docker ps
列出执行中的容器

docker ps -a
option:
-a : 列出所有容器包括未启动的
```
列出容器和IMAGE
```
docker container list
docker container list --all
docker image list
docker image list --all
```
### 容器启动
```
docker start [container Id]
```
### 容器停止
```
docker stop [container Id]
```
### 进入容器
```
docker exec [container Id] -it bash
```
### 强行中止
```
docker kill [container Id]
```
### 容器删除
```
docker rm [container Id]
```
# docker-compose
## 查看docker-compose容器
```
docker-compose ps             #与doker ps 不同，只列出容器名，不列出容器和镜像ID
docker-compose ps --services  #只列出service name(docker-compose文件中定义的service name)
docker-compose config         #查看 docker-compose文件内容
```

```
docker-compose up
```
options:
```
-d
```
```
docker-compose down
```
```
docker-compose bulid
```
options:
```
--no-cache
```
```
docker-compose exec [servicename]
```

彻底清除所有镜像和容器
```
docker-compose down                       #docker-compose 停止
docker rm $(docker ps -a -q)              #清除所有容器（windows下可用Powershell 执行）
docker rmi $(docker images -q)            #清除所有镜像（windows下可用Powershell 执行）
docker volume rm $(docker volume ls -q)   #清除所有volume（windows下可用Powershell 执行）
```



