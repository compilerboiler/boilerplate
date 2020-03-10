---
title: simple python-example-30 (snippet)
date: 2020-02-10
tags: ["python"]
---
Python example 'python-example-30'


## python-example-30

Python example: python-example-30

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

a = int(raw_input("请输入一个数字:\n"))
x = str(a)
flag = True

for i in range(len(x)/2):
    if x[i] != x[-i - 1]:
        flag = False
        break
if flag:
    print("%d 是一个回文数!" % a)
else:
    print("%d 不是一个回文数!" % a)


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
