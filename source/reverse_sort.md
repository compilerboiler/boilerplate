---
title: reverse sort (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'reverse sort'

Functions in program: 
* def reverse_sort(array):

## reverse sort

Python beginners example: reverse sort

```python
"""
This sort is designed by me.
First self designed sorting Algorithm.
Kalpak Take
"""

def reverse_sort(array):
	for i in range(len(array) - 1):
		for n in range(len(array) - 1):
			a = array[n]
			if (a < array[i]):
				tem = array[i]
				array[i] = a 
				array[n] = tem 
	return array			
	
print(reverse_sort([123, 3455, 6577, 546, 345, 22, 56, 7])	)


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
- Another Python site: https://pythonprogramminglanguage.com
