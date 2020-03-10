---
title: simple python-example-40 (snippet)
date: 2020-02-10
tags: ["python"]
---
Python example 'python-example-40'


## python-example-40

Python example: python-example-40

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

if __name__ == '__main__':
    a = [9,6,5,4,1]
    N = len(a) 
    print(a)
    for i in range(len(a) / 2):
        a[i],a[N - i - 1] = a[N - i - 1],a[i]
    print(a)


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
