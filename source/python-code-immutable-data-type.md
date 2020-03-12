---
title: python-code-immutable-data-type (snippet)
date: 2020-02-15
tags: ["python"]
---
Python example 'python-code-immutable-data-type'


## python-code-immutable-data-type

Python code example: python-code-immutable-data-type

```python
>>> a = [1, 2, 4, 8, 16] >>> a[0] = 32 # OK. You can modify lists.
>>> a
[32, 2, 4, 8, 16]
>>> a = (1, 2, 4, 8, 16)
>>> a[0] = 32 # Wrong! You can't modify tuples.
Traceback (most recent call last):
File "", line 1, in
TypeError: 'tuple' object does not support item assignment


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org

More Python: https://pythonprogramminglanguage.com
