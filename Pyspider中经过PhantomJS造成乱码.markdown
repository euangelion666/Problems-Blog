﻿# Pyspider中经过PhantomJS造成乱码

标签（空格分隔）： Pyspider

---

在crawl时设置fetch_type='js'，使得网页通过PhantomJS运行js语句，但是有的页面会出现乱码的情况，这里可能会与headers的设置有关，传入一个空headers可能会有所帮助，如果必须要传入headers，可能需要不断尝试找到最合适的参数




