---
title: linear search (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'linear search'. This program is an example of the linear search algorithm.

Functions in program: 
* `def linear_search(array, to_find):`

## linear search

Python beginners example: linear search

```python
# Linear Search or Sequential Search Algorithm

def linear_search(array, to_find):
	pos = 0			# Starting position or index
	to_return = (False, 0)
	while (pos < len(array)):		# while index is less than length of array
		if (array[pos] == to_find):		# if array with index of var pos is equal to find
			to_return = (True, pos)			# no need to break loop cuz return appends func
			return to_return
		else: 
			pos = pos + 1		# if elem not found continue to next pos 
	return to_return
	
nums = [12, 34, 54, 88, 21]			
print(linear_search(nums, 88)			)

```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
