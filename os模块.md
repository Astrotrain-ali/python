# os模块
---

-   getcwd 获取当前工作目录
```
import os

print(os.getcwd())
```
-   chdir 切换当前目录
```
import os

print(os.getcwd())
os.chdir("ali")
print(os.getcwd())
```
-  mkdir 创建单级目录
```
os.mkdir("ali1")
```
-  mkdirs 创建多层级目录
```
os.mkdirs("ali1/ali2")
```
-  removedirs 删除空目录,如果目录不为空则无法删除
```
import os

print(os.getcwd())
os.removedirs("ali/ali1/ali2")
```

-  listdir 列出当前目录下所有文件和目录
```
import os

print(os.listdir())

```
-   stat 显示文件元数据
```
import os

print(os.stat("nginx.conf"))
```
-   join 路径拼接
```
import os

a = "/Users/mutantbox/PycharmProjects"
b = "untitled/test.py"
print(os.path.join(a,b))
```
 