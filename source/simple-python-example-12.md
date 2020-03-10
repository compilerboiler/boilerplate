---
title: simple python-example-12 (snippet)
date: 2020-02-10
tags: ["python"]
---
Python example 'python-example-12'


## python-example-12

Python example: python-example-12

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

h = 0
leap = 1
from math import sqrt
from sys import stdout
for m in range(101,201):
    k = int(sqrt(m + 1))
    for i in range(2,k + 1):
        if m % i == 0:
            leap = 0
            break
    if leap == 1:
        print('%-4d' % m)
        h += 1
        if h % 10 == 0:
            print('')
    leap = 1
print('The total is %d' % h)


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
