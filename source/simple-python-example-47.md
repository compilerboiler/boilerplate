---
title: simple python-example-47 (snippet)
date: 2020-02-10
tags: ["python"]
---
Python example 'python-example-47'

Functions in program: 
* `def exchange(a,b):`

## python-example-47

Python example: python-example-47

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

def exchange(a,b):
    a,b = b,a
    return (a,b)

if __name__ == '__main__':
    x = 10
    y = 20
    print('x = %d,y = %d' % (x,y))
    x,y = exchange(x,y)
    print('x = %d,y = %d' % (x,y))


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
