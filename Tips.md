
# Database
## MySql
#### Mysql Version 确认
```
方法1 ： mysql -V
方法2 ： select version()
```
#### Schema 确认
```
显示数据库
show databases;
```
```
显示表
show tables;
```
```
显示Database DDL
show create database {database name};

```
# Go
### GO依赖Package的管理
glide 的使用说明
Go1.5以前需要设定一个环境变量,来使用vendor目录
```
//设置环境变量 使用vendor目录
GO15VENDOREXPERIMENT=1
```
Go1.6以后默认启用变量，Go1.7 移除变量加入标准中
Glide 从概念上来讲是一个 Go 的包管理工具，类似于 Rust 的 Cargo， 
Node.js 的 NPM，Python 的 Pip，Ruby 的 Boundler 等，Java的Maven和Gradle。
Go语言也有众多的依赖包管理工具，glide是其中比较出众的一个。
glide工具可以解析import（估计这也是Go编译器不允许import中存在未使用的依赖包的原因），
生成依赖关系树到lock文件中。然后拉取依赖包文件到vendor目录下。

安装glide
```
$ go get github.com/Masterminds/glide
$ go install github.com/Masterminds/glide
```
Windows,Mac下：[下载安装文件](https://github.com/Masterminds/glide/releases)
# NodeJs
## PM2
## NPM
# C#
# Docker
# SQL
# JAVA
# JAVASCRIPT
# CSS
# Git
# ubuntu
## Hyper-V 上变更显示器分辨率
```
1. $sudoedit /etc/default/grub
2. 编辑
GRUB_CMDLINE_LINUX_DEFAULT="quiet splash video=hyperv_fb:920x1080"
#如果Hyper-V里添加了RemoteFx3D Vedio 要删除，因为ubuntu不支持
#编辑完成后Ctrl+X保存
3.sudo update-grub
4.reboot
```

