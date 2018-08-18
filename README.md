# Docker 笔记
## Docker 常用命令
管理容器
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
### 容器中止
```
docker kill [container Id]
```
### 容器清除
```
docker rm [container Id]
```

