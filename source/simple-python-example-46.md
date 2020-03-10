---
title: simple python-example-46 (snippet)
date: 2020-02-10
tags: ["python"]
---
Python example 'python-example-46'

Functions in program: 
* `def SQ(x):`

## python-example-46

Python example: python-example-46

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

TRUE = 1
FALSE = 0
def SQ(x):
    return x * x
print('如果输入的数字小于 50，程序将停止运行。')
again = 1
while again:
    num = int(raw_input('Please input number'))
    print('运算结果为 %d' % (SQ(num)))
    if num >= 50:
        again = TRUE
    else:
        again = FALSE


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
