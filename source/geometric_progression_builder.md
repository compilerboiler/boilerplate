---
title: geometric progression builder (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'geometric progression builder'

Functions in program: 
* def build_geo_sequence(start, end, constant):

## geometric progression builder

Python beginners example: geometric progression builder

```python
"""
Simply it just builds a geometric progression on given conditions.
Iterates through t1 till n 
multiplies last values in list to constant
append it back to list 
COOL!
"""

def build_geo_sequence(start, end, constant):
	temp = [start]
	try:
		for i in range(start, end):
			temp.append(temp[-1] * constant)
	except TypeError as te:
		print(te)
	except Exception as e:
		print(e)
	else:
		return temp

# Test 
res = build_geo_sequence(1, 10, 3)
print("Geo Sequence:")
for i in res:
	print("  " + str(i))
# Expected -> 1, 3, 9, 27, 81, ....
# Here a = 1, d = 3


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
- Another Python site: https://pythonprogramminglanguage.com
