---
title: kay sort (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'kay sort'

Functions in program: 
* `def kay_sort(array):`

## kay sort

Python beginners example: kay sort

```python
"""
This sort is same as reverse sort by me.
Except minor changes in first for loop, and
comparison sign on line 11
And function is called kay_sort because
kay is my nickname
"""

def kay_sort(array):
	print("Orignal List : {}".format(array))
	for i in range(len(array)):
		for n in range(len(array) - 1):
			a = array[n]
			if (a > array[i]):
				tem = array[i]
				array[i] = a 
				array[n] = tem 
	return "Sorted List : {}".format(array)			
	
print(kay_sort([123, 4, 123, 4])	)


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
