---
title: simple python-example-37 (snippet)
date: 2020-02-11
tags: ["python"]
---
Python example 'python-example-37'


## python-example-37

Python example: python-example-37

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

if __name__ == "__main__":
    N = 10
    # input data
    print('please input ten num:\n')
    l = []
    for i in range(N):
        l.append(int(raw_input('input a number:\n')))
    print
    for i in range(N):
        print(l[i])
    print

    # sort ten num
    for i in range(N - 1):
        min = i
        for j in range(i + 1,N):
            if l[min] > l[j]:min = j
        l[i],l[min] = l[min],l[i]
    print('after sorted')
    for i in range(N):
        print(l[i])


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
