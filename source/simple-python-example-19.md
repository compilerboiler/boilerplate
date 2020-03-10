---
title: simple python-example-19 (snippet)
date: 2020-02-11
tags: ["python"]
---
Python example 'python-example-19'


## python-example-19

Python example: python-example-19

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

from sys import stdout
for j in range(2,1001):
    k = []
    n = -1
    s = j
    for i in range(1,j):
            if j % i == 0:
                n += 1
                s -= i
                k.append(i)
    
    if s == 0:
        print(j)
        for i in range(n):
            stdout.write(str(k[i]))
            stdout.write(' ')
        print(k[n])


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
