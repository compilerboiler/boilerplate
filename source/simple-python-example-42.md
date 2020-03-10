---
title: simple python-example-42 (snippet)
date: 2020-02-11
tags: ["python"]
---
Python example 'python-example-42'

Functions in program: 
* `def autofunc():`

## python-example-42

Python example: python-example-42

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

num = 2
def autofunc():
    num = 1
    print('internal block num = %d' % num)
    num += 1
for i in range(3):
    print('The num = %d' % num)
    num += 1
    autofunc()


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
