﻿# pycurl安装

标签（空格分隔）： Python3

---
pip可以直接安装，但是安装之后import可能会出现一下报错
```Python
ImportError: pycurl: libcurl link-time ssl backend (openssl) is different from compile-time ssl backend (none/other)
```
    
解决方法是：

+ 卸载pycurl
```bash
pip uninstall pycurl
```
    
+ 在bash或你所使用的终端中，设置pycurl的ssl库
```bash
export PYCURL_SSL_LIBRARY=openssl
# 这里值与报错中的显示有关
# libcurl link-time ssl backend (openssl)
# 设置PYCURL_SSL_LIBRARY的值与上面括号中的值一致
```
+ 再次安装pycurl
```bash
pip install pycurl
```

    
    




