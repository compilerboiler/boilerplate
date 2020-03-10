---
title: simple python-example-22 (snippet)
date: 2020-02-10
tags: ["python"]
---
Python example 'python-example-22'


## python-example-22

Python example: python-example-22

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

for i in range(ord('x'),ord('z') + 1):
    for j in range(ord('x'),ord('z') + 1):
        if i != j:
            for k in range(ord('x'),ord('z') + 1):
                if (i != k) and (j != k):
                    if (i != ord('x')) and (k != ord('x')) and (k != ord('z')):
                        print('order is a -- %s\t b -- %s\tc--%s' % (chr(i),chr(j),chr(k)))


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
