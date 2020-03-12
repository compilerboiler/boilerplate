---
title: python-code-immutable-data-type-2 (snippet)
date: 2020-02-15
tags: ["python"]
---
Python example 'python-code-immutable-data-type-2'


## python-code-immutable-data-type-2

Python code example: python-code-immutable-data-type-2

```python
>>> # Lists (mutable)
>>> a = [1, 2, 4] # a is a list
>>> b = a # a and b refer to the same list object
>>> id(a) == id(b)
True
>>> a += [8, 16] # a is modified and so is b - they refer to the same object
>>> a
[1, 2, 4, 8, 16]
>>> b
[1, 2, 4, 8, 16]
>>> id(a) == id(b)
True
>>>
>>> # Tuples (immutable)
>>> a = (1, 2, 4) # a is a tuple
>>> b = a # a and b refer to the same tuple object
>>> id(a) == id(b)
True
>>> a += (8, 16) # new tuple is created and assigned to a; b is unchanged
>>> a # a refers to the new object
(1, 2, 4, 8, 16)
>>> b # b refers to the old object
(1, 2, 4)
>>> id(a) == id(b)
False


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org

More Python: https://pythonprogramminglanguage.com
