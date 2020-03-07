---
title: enum (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'enum'

Functions in program: 
* `def enum(ar):`

## enum

Python beginners example: enum

```python
#!/usr/bin/python
# -*- coding: utf-8 -*-

# Enum function
# yields a tuple of element and it's index
def enum(ar):
	for index in range(len(ar)):
		yield((index, ar[index]))

# Test
case_1 = [19, 17, 20, 23, 27, 15]
for tup in list(enum(case_1)):
	print(tup)


# Enum function is a generator does not 
# return any value, instead generates
# tuple as it encounters element of array

# Tuples can be appended to list
# and can be returned after iteration
# However,
# Generator is a good option


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
