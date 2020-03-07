---
title: item index (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'item index'

Functions in program: 
* `def index(array, item):`

## item index

Python beginners example: item index

```python
"""Algorithm for finding index of element in an array"""

def index(array, item):
	index = 0
	found = False
	while (not found):
		if (array[index] == item):
			found = True
		else:
			index = index + 1
	return index 

print(index([12, 34], 34)	)

```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
