---
title: simple python-example-14 (snippet)
date: 2020-02-10
tags: ["python"]
---
Python example 'python-example-14'


## python-example-14

Python example: python-example-14

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

from sys import stdout
n = int(raw_input("input number:\n"))
print("n = %d" % n)

for i in range(2,n + 1):
    while n != i:
        if n % i == 0:
            stdout.write(str(i))
            stdout.write("*")
            n = n / i
        else:
            break
print("%d" % n)


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
