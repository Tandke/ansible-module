# ansible-module

## 简介
ansible一些常用的自动配置模块：
* system-init：用于初始化操作系统，目前支持CentOS7、Ubuntu16.04、Ubuntu18.04
* kubernetes：用于安装kubernetes，需要自行提供kubernetes的安装包，支持quagga和flannel两种网络插件
* moosefs：用于安装moosefs分布式文件系统

> 需要使用ansible2.2以上版本


## 安装ansible
下面是ansible的基本安装:

ubuntu：

```
$ sudo apt-get install software-properties-common
$ sudo apt-add-repository ppa:ansible/ansible
$ sudo apt-get update
$ sudo apt-get install ansible
```

centos：

```
yum install ansible
```
> 使用yum安装，需要额外配置epel源，否则安装的ansible版本会比较旧

## 使用

安装好ansible以后，直接将该项目clone至/etc/ansible目录，并将其重命名为roles即可。

将目录下的ansible.cfg复制到/etc/ansible/目录下，覆盖默认的配置文件。
