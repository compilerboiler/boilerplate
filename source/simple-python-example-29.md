---
title: simple python-example-29 (snippet)
date: 2020-02-11
tags: ["python"]
---
Python example 'python-example-29'


## python-example-29

Python example: python-example-29

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

x = int(raw_input("请输入一个数:\n"))
a = x / 10000
b = x % 10000 / 1000
c = x % 1000 / 100
d = x % 100 / 10
e = x % 10

if a != 0:
    print("5 位数：",e,d,c,b,a)
elif b != 0:
    print("4 位数：",e,d,c,b,)
elif c != 0:
    print("3 位数：",e,d,c)
elif d != 0:
    print("2 位数：",e,d)
else:
    print("1 位数：",e )


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
