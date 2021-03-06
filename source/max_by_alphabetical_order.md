---
title: max by alphabetical order (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'max by alphabetical order'

Functions in program: 
* `def max_alphabetical_order(s):`
* `def lower_(arr):`

Modules used in program: 
* `import string `

## max by alphabetical order

Python beginners example: max by alphabetical order

```python

import string 

def lower_(arr):
	"""
	For conversion of every element in list to lower 
	"""
	for i in range(len(arr)):
		arr[i] = arr[i].lower()

def max_alphabetical_order(s):
	"""
	Useful on lists containing strings that start from alphabets,
	because the algorithm is written for it in the first place!
	"""
	copy = s[:]
	useful = list(string.ascii_lowercase)
	lower_(s)
	res = s[0]
	for word in s[1:]:
		tmp = word[0]
		if useful.index(tmp) > useful.index(res[0]):
			res = word
	return copy[s.index(res)]
	
# Test
case1 = ["Alpha", "Beta", "Gist", "exotic", "hells kitchen", "word", "Ultra", "zip"]
call = max_alphabetical_order(case1)
print("Max element in list by alphabet order:\n" + call)


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
