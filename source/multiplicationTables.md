---
title: multiplicationTables (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'multiplication Tables'. This snippet outputs multiplication tables.

## multiplicationTables

Python beginners example: multiplicationTables

```python
# Multiplication Table viewer

while True:
	startOrEnd = str(input('Start or End : '))
	if startOrEnd == 'Start':
		whichTable = int(input('Which Table : '))
		for x in range(1, 13):
			table =  whichTable * x
			print(table)
		continue
	else :
		print('Program Ended...')
		break	


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
