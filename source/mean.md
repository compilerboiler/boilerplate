---
title: mean (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'mean'

Functions in program: 
* `def mean_ar(ar):`
* `def mean_(*args):`

## mean

Python beginners example: mean

```python
#!/usr/bin/python
# -*- coding: utf-8 -*-

# f(x) = s(x) / l(x) ______(e1)
# Functions below same principle as (e1)
#
# Here,
# Mean value can be float
# 'er is need to declare float values

# Function to get mean of given args
def mean_(*args):
	sum_ = 0.0
	length_ = 0.0

	for arg in args:
		sum_ += arg
		length_ += 1.0

	return sum_ / length_

# Function to get mean of array
def mean_ar(ar):
	return float(sum(ar))/float(len(ar))

# Another feature can be start index
# and end index of array

# Test
# First function
if mean_(12, 445, 76, 23, 7, 9, 17, 19, 100) == 78.66666666666667:
	print("First Function Works!")

# Second function
if mean_ar([12, 445, 76, 23, 7, 9, 17, 19, 10]) == 68.66666666666667:
	print("Second Function Works!")



```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
