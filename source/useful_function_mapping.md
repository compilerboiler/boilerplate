---
title: useful function mapping (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'useful function mapping'

Functions in program: 
* `def is_odd(n):`
* `def is_even(n):`
* `def is_divisible(n, t):`
* `def raise_power(n, power):`
* `def cubed(n):`
* `def squared(n):`

## useful function mapping

Python beginners example: useful function mapping

```python
#!/usr/bin/python
# -*- coding: utf-8 -*-

def squared(n):
	return n * n 

def cubed(n):
	return n * n * n 

def raise_power(n, power):
	for t in range(power):
		n *= n 
	return n 

def is_divisible(n, t):
	return n % t == 0

def is_even(n):
	return n % 2 == 0

def is_odd(n):
	return n % 2 != 0

# These all functions are extremely 
# helpful when used with map method of python
# map(func, list) basically applies given function 
# to every element of list and appends results to a new
# list

# e.g.
print(map(squared, [1, 3, 5, 7, 9, 11, 13, 15]))

# for functions with multiple args
# see: https://www.quora.com/How-do-I-put-multiple-arguments-into-a-map-function-in-Python



```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
