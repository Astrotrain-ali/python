# range

---

**将文字对应的索引打印出来**

    1
    2
    3
    4
    5
    #!/usr/bin/env python
    # _*_ coding:utf-8 _*_
    test = input(">>>")
    for i in range(0, len(test)):
        print(i, test[i])
　　

**帮助创建连续的数字，通过设置步长来指定不连续**
 

    1
    2
    3
    v = range(0, 100, 5)
    ror item in v:
    print(item)
