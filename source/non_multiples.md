---
title: non multiples (snippet)
date: 2019-02-07
tags: ["python"]
---

## non multiples

Python beginners example: non multiples

```python
number_to_check = int(input("Number : "))
till_where = int(input("Till where to check : "))
list_of_non_multiples = []
for num in range(0, till_where + 1):
	if num % number_to_check != 0:
		list_of_non_multiples.append(num)
		
print(list_of_non_multiples)
# or you can do 
# this
print(" ")
for element in list_of_non_multiples:
	print(element)


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
