---
title: ordered binary search (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'ordered binary search'

Functions in program: 
* def Ordered_binary_search(arra, elem):
* def binary_search(array, n):

## ordered binary search

Python beginners example: ordered binary search

```python
def binary_search(array, n):
	arr = sorted(array)
	to_return = False 
	first_elem = 0
	last_elem = len(arr) - 1
	while (first_elem <= last_elem):
		mid = (first_elem + last_elem) // 2
		if (arr[mid] == n):
			to_return = True
			break
		else:
			if (n > arr[mid]):
				first_elem = mid + 1
			else:
				last_elem = mid - 1
	return to_return			


def Ordered_binary_search(arra, elem):
	if (len(arra) == 0):
		return False
	
	middle = len(arra) // 2	
	if (arra[middle] == elem):
		return True 
	else:	
		if (elem > arra[middle]):
			return binary_search(arra[middle:], elem)
		else: 
			return binary_search(arra[:middle], elem) 	
		
nums = [0,23,54,5,32,78]	
print(Ordered_binary_search(nums, 32)	)
print(Ordered_binary_search(nums, 5)	)


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
- Another Python site: https://pythonprogramminglanguage.com
