﻿# CentOS上安装Python3的方法

标签（空格分隔）： CentOS

---

### 1.编译安装
+ 依赖包安装
```bash
yum groupinstall development  
yum install openssl-devel sqlite-devel bzip2-devel gdbm-devel
ncurses-devel xz-devel readline-devel  
```
+ 下载编译包 [Python编译包下载地址](https://www.python.org/downloads/)
+ 解压，进入文件夹
+ 编译安装[^footnote]
```bash
./configure --prefix=/安装位置
make
make install
```
[^footnote]: 这里遇上过无限循环make的情况，解决方法是矫正系统时间

+ 配置命令[^footnote2]
```bash
ln -s /安装目录/bin/python3 /usr/bin/python3  
```
[^footnote2]:这里注意是否有系统自带的命令，如果有注意千万不要覆盖

### 2. yum安装
未完待续
