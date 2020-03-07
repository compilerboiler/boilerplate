---
title: number lesser greater (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'number lesser greater'

Functions in program: 
* `def pos_neg_zero(x): `

Modules used in program: 
* import sys

## number lesser greater

Python beginners example: number lesser greater

```python

import sys

# Use of 
# Conditionals in python
# Determines weather the number is positive negative or zero
def pos_neg_zero(x): 
	if x < 0:  return "Negative" 
	elif x > 0:  return "Positive" 
	return "Zero"

while True:
	if str(raw_input(" Start [Y/n]?  ")).strip().lower()== "y":
		print("    [Num] = " + pos_neg_zero(float(raw_input(" Number:  "))) + "\n")
	else:
		print("Bye!")
		sys.exit(0)


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
