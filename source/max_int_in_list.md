---
title: max int in list (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'max int in list'. Finds the maximum number in a list.

Functions in program: 
* `def convert():`
* `def compare(li):`

## max int in list

Python beginners example: max int in list

```python

def  compare(li):
	res = 0
	for i in range(len(li) - 1):
		a = li[i]
		b = li[i + 1]
		if (a > b):
			if (a > res):
				res = a 
		else:
			if (b > res):
				res = b	
	return res 
	
def convert():	
	get_input = raw_input("Enter Space Seperated Numbers : ")
	raw = get_input.split()
	nums = []
	for i in raw:
		nums.append(float(i))
	return nums

if __name__ == "__main__":	
	print(compare(convert()))

```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
