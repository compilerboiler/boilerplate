---
title: simple python-example-89 (snippet)
date: 2020-02-10
tags: ["python"]
---
Python example 'python-example-89'


## python-example-89

Python example: python-example-89

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

from sys import stdout
if __name__ == '__main__':
    a = int(raw_input('input a number:\n'))
    aa = []
    aa.append(a % 10)
    aa.append(a % 100 / 10)
    aa.append(a % 1000 / 100)
    aa.append(a / 1000)

    for i in range(4):
        aa[i] += 5
        aa[i] %= 10
    for i in range(2):
        aa[i],aa[3 - i] = aa[3 - i],aa[i]
    for i in range(3,-1,-1):
        stdout.write(str(aa[i]))


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com