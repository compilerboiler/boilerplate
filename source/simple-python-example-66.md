---
title: simple python-example-66 (snippet)
date: 2020-02-10
tags: ["python"]
---
Python example 'python-example-66'


## python-example-66

Python example: python-example-66

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

if __name__ == '__main__':
    n1 = int(raw_input('n1 = :\n'))
    n2 = int(raw_input('n2 = :\n'))
    n3 = int(raw_input('n3 = :\n'))

    def swap(p1,p2):
        return p2,p1

    if n1 > n2 : n1,n2 = swap(n1,n2)
    if n1 > n3 : n1,n3 = swap(n1,n3)
    if n2 > n3 : n2,n3 = swap(n2,n3)

    print(n1,n2,n3)


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com