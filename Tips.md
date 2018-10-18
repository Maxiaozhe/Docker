
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
# linux
# Windows
## remote desktop 
### surface上显示文字过小的问题
操作步步骤
1.编辑下列文件，存到 mstsc.manifest文件中（UTF-8）
```
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<assembly xmlns="urn:schemas-microsoft-com:asm.v1" manifestVersion="1.0" xmlns:asmv3="urn:schemas-microsoft-com:asm.v3">
<dependency>
  <dependentAssembly>
    <assemblyIdentity
      type="win32"
      name="Microsoft.Windows.Common-Controls"
      version="6.0.0.0" processorArchitecture="*"
      publicKeyToken="6595b64144ccf1df"
      language="*">
    </assemblyIdentity>
  </dependentAssembly>
</dependency>

<dependency>
  <dependentAssembly>
    <assemblyIdentity
      type="win32"
      name="Microsoft.VC90.CRT"
      version="9.0.21022.8"
      processorArchitecture="amd64"
      publicKeyToken="1fc8b3b9a1e18e3b">
    </assemblyIdentity>
  </dependentAssembly>
</dependency>

<trustInfo xmlns="urn:schemas-microsoft-com:asm.v3">
  <security>
    <requestedPrivileges>
      <requestedExecutionLevel
        level="asInvoker"
        uiAccess="false"/>
    </requestedPrivileges>
  </security>
</trustInfo>

<asmv3:application>
  <asmv3:windowsSettings xmlns="http://schemas.microsoft.com/SMI/2005/WindowsSettings">
    <ms_windowsSettings:dpiAware xmlns:ms_windowsSettings="http://schemas.microsoft.com/SMI/2005/WindowsSettings">false</ms_windowsSettings:dpiAware>
  </asmv3:windowsSettings>
</asmv3:application>
</assembly>
```
2.修改注册表，使得manifast设置生效

3.系统重启
## ubuntu
### 系统设置
#### Hyper-V 上变更显示器分辨率
```
1. $sudoedit /etc/default/grub
2. 编辑
GRUB_CMDLINE_LINUX_DEFAULT="quiet splash video=hyperv_fb:920x1080"
#如果Hyper-V里添加了RemoteFx3D Vedio 要删除，因为ubuntu不支持
#编辑完成后Ctrl+X保存
3.sudo update-grub
4.reboot
```
### 常用命令
#### 执行sh批处理文件
```
sudo sh shcommand.sh
```

