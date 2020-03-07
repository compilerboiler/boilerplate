---
title: difference testing (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'difference testing'

Functions in program: 
* def find_difference_matching(x , y , diff = 0):

## difference testing

Python beginners example: difference testing

```python
# We assume that the input always be find_difference_matching(list, list, integer)
def find_difference_matching(x , y , diff = 0):
	res = []
	for i in range(len(x)):
	    if abs(x[i] -  y[i]) == diff:
		    res.append((x[i], y[i]))
	return res

# Test
a = [12, 10, 123, 76, 9990]
b = [2, 0, 45,66, 10000]
result = find_difference_matching(a, b, 10)
print("Matches:")
for i in result:
    print("   " + str(i))


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
- Another Python site: https://pythonprogramminglanguage.com
