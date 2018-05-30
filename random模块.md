# random模块
---
#### random模块验证码功能
```
import random

def v_code():
    ret = ""
    for i in range(5):
        num = random.randint(0,9)
        alf = chr(random.randint(66,122))
        s = str(random.choice([num,alf]))
        ret += s
    return ret
print(v_code())

```




