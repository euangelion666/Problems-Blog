﻿# cx_Oracle插入中文乱码

标签（空格分隔）： Python3 Oracle

---

需要同时设置Python中NLS_LANG的值，和bash中oracle的NLS
_LANG的值

Python
```Python
import os
os.environ['NLS_LANG'] = 'SIMPLIFIED CHINESE_CHINA.UTF8'  
```

Bash
```bash
cd /home/oracle/ #这里要进入oracle用户的目录下
vi .bash_profile
    插入NLS_LANG="SIMPLIFIED CHINESE_CHINA.UTF8";export NLS_LANG
source .bash_profile
```
    



