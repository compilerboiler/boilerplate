---
title: python code python-code-recursive-functions (snippet)
date: 2019-02-15
tags: ["python"]
---
Python example 'python code python-code-recursive-functions'


## python code python-code-recursive-functions

Python code example: python code python-code-recursive-functions

```python
>>> def factorial_r(n):
if n == 0:
return 1
return n * factorial_r(n - 1)
>>>
>>> def factorial_l(n):
if n == 0:
return 1
product = 1
for i in range(1, n+1):
product *= i
return product


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org

More Python: https://pythonprogramminglanguage.com
