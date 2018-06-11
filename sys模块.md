# sys模块
---

-   sys.argv #命令行参数list,第一个元素是程序本身路径
-   sys.exit(n) #退出程序，正常退出时exit(0)
-   sys.version #获取python解释程序的版本信息
-   sys.maxint #最大的int值
-   sys.path #返回模块的搜索路径，初始化时使用pythonpath环境变量的值
-   sys.platform #返回操作系统平台名称
-   sys.stdout #进度条
```
import sys
import time


for i in range(100):
    sys.stdout.write("#")
    time.sleep(0.5)
    sys.stdout.flush()
```



