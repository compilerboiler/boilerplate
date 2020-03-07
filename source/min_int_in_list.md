---
title: min int in list (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'min int in list'

Functions in program: 
* def convert():	
* def  compare(li):

## min int in list

Python beginners example: min int in list

```python

def  compare(li):
	if (len(li) == 1):
		return "Single Value To Compare {} in List".format(li[0])
	res = 0
	for i in range(len(li) - 1):
		a = li[i]
		b = li[i + 1]
		if (a < b):
			if (i != 0): 
				if (a < res):
					res = a
			else:
				res = a 	
		else:
			if (i != 0):
				if (b < res):
					res = b
			else:
				res = b	
	return res 
	
def convert():	
	get_input = raw_input("Enter Space Seperated Numbers : ")
	raw = get_input.split()
	nums = []
	for i in raw:
		nums.append(float(i))
	return nums

if __name__ == "__main__":	
	print(compare(convert())		)


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
- Another Python site: https://pythonprogramminglanguage.com
