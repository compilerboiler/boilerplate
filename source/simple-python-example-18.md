---
title: simple python-example-18 (snippet)
date: 2020-02-11
tags: ["python"]
---
Python example 'python-example-18'


## python-example-18

Python example: python-example-18

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

Tn = 0
Sn = []
n = int(raw_input('n = :\n'))
a = int(raw_input('a = :\n'))
for count in range(n):
    Tn = Tn + a
    a = a * 10
    Sn.append(Tn)
    print(Tn)

Sn = reduce(lambda x,y : x + y,Sn)
print(Sn)


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
