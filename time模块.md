# time模块
---
-   时间戳
```
import time

print(time.time())
```
-   当地时间
```
import time

print(time.localtime())

t = time.localtime()

print(t.tm_year)
print(t.tm_mon)
print(t.tm_mday)
```
-   世界标准时间（utc）
```
import
print(time.gmtime())
```
-   结构化时间转换时间戳
```
import time

print(time.mktime(time.localtime()))
```
-   结构化时间转换字符串时间
```
import time

print(time.strftime("%Y-%m-%d-%X",time.localtime()))
```
-   字符串时间转换为结构化时间
```
import time

print(time.strptime("2018:05:28:18:18:18","%Y:%m:%d:%X"))
```
-   直观的显示时间
```
print(time.asctime())
print(time.ctime())
```
- datetime
```
import datetime
print(datetime.datetime.now())
```