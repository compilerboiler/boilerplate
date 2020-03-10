---
title: simple python-example-6 (snippet)
date: 2020-02-10
tags: ["python"]
---
Python example 'python-example-6'

Functions in program: 
* `def fib(n):`

## python-example-6

Python example: python-example-6

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

def fib(n):
	a,b = 1,1
	for i in range(n-1):
		a,b = b,a+b
	return a

# 输出了第10个斐波那契数列
print(fib(10))


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
