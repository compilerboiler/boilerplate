---
title: simple python-example-2 (snippet)
date: 2020-02-10
tags: ["python"]
---
Python example 'python-example-2'


## python-example-2

Python example: python-example-2

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

i = int(raw_input('净利润:'))
arr = [1000000,600000,400000,200000,100000,0]
rat = [0.01,0.015,0.03,0.05,0.075,0.1]
r = 0
for idx in range(0,6):
    if i>arr[idx]:
        r+=(i-arr[idx])*rat[idx]
        print((i-arr[idx])*rat[idx])
        i=arr[idx]
print(r)


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com