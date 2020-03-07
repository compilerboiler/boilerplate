---
title: binary to decimal converter (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'binary to decimal converter'

Functions in program: 
* def binary_to_decimal_conv(binary_string):

Modules used in program: 
* import sys

## binary to decimal converter

Python beginners example: binary to decimal converter

```python
#!/usr/bin/python
# -*- coding: utf-8 -*-


import sys

# Binary to decimal conversion
# See explaination: https://i.imgur.com/heAT0PB.gif   , 
# https://www.electronics-tutorials.ws/binary/bin_2.html

# Pesudo code:
# Iterate through binary num
# if 0 then pass
# else result = result + bit(1) * 2 ** index of bit(1)

def binary_to_decimal_conv(binary_string):
	res = 0
	binary_l = list(binary_string)
	for bit_i in range(len(binary_l)):
		res += int(binary_l[bit_i]) * (2 ** bit_i) 
	return res 

# Test
# Testing interface
i = 0
while True:
	if raw_input("\n[{}] Exit(press e) or Continue(press c): ".format(i)).strip().lower() == "c":
		print("Decimal form: " + str(binary_to_decimal_conv(raw_input("\nBinary?: "))))
	else:
		print("\nHope you enjoyed!")
		sys.exit()
	i += 1


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
- Another Python site: https://pythonprogramminglanguage.com
