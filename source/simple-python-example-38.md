---
title: simple python-example-38 (snippet)
date: 2020-02-11
tags: ["python"]
---
Python example 'python-example-38'


## python-example-38

Python example: python-example-38

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

if __name__ == '__main__':
    a = []
    sum = 0.0
    for i in range(3):
        a.append([])
        for j in range(3):
            a[i].append(float(raw_input("input num:\n")))
    for i in range(3):
        sum += a[i][i]
    print(sum)


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
