---
title: simple python-example-27 (snippet)
date: 2020-02-11
tags: ["python"]
---
Python example 'python-example-27'

Functions in program: 
* `def output(s,l):`

## python-example-27

Python example: python-example-27

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

def output(s,l):
    if l==0:
       return
    print((s[l-1]))
    output(s,l-1)
 
s = raw_input('Input a string:')
l = len(s)
output(s,l)


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
