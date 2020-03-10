---
title: simple python-example-26 (snippet)
date: 2020-02-11
tags: ["python"]
---
Python example 'python-example-26'

Functions in program: 
* `def fact(j):`

## python-example-26

Python example: python-example-26

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

def fact(j):
    sum = 0
    if j == 0:
        sum = 1
    else:
        sum = j * fact(j - 1)
    return sum

for i in range(5):
    print('%d! = %d' % (i,fact(i)))


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
