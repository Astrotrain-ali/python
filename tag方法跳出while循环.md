# tag方法跳出while循环
---
```
tag = True
while tag:
    print('level1')
    choice = input('level1>:')
    if choice == 'quit':break
    if choice == 'quit_all':tag = False
    while tag:
        print('level2')
        choice = input('level2>:')
        if choice == 'quit': break
        if choice == 'quit_all':tag = False
        while tag:
            print('level3')
            choice = input('level3>:')
            if choice == 'quit': break
            if choice == 'quit_all':tag = False
```




