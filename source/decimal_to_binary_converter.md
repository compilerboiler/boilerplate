---
title: decimal to binary converter (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'decimal to binary converter'

Functions in program: 
* def decimal_to_binary(n):
* def concat(S):

## decimal to binary converter

Python beginners example: decimal to binary converter

```python
# For concatenation
def concat(S):
	res = ""
	for i in S:
		if not isinstance(i, str):
			res += str(i)
		else:
			res += i
	return res 

# Simple Base 10 number(Decimal) number converter to Base 2 number(binary) number
# Function returns answer in str datatype
# For understanding steps: http://www.electronics-tutorials.ws/binary/bin_2.html
def decimal_to_binary(n):
	res = []
	while n != 0:
		res.append(n % 2)
		n = n // 2
	final = concat(res) + "0"
	return final[::-1]


# Test
cases = [123, 23455, 253552, 87985, 3479434, 76, 246572, 231, 69, 2, 7, 2, 543]
for case in cases:
	built_in = str(bin(case))[2:]
	my_func = decimal_to_binary(case)[1:] # For test purposes
	if built_in == my_func:
		print("Decimal: " + str(case))
		print("Binary: " + my_func + "\nTest Passed!\n")
	else:
		print("Test Failed! Badly!!\n")


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
- Another Python site: https://pythonprogramminglanguage.com
