---
title: sum of arithmetic sequence (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'sum of arithmetic sequence'


## sum of arithmetic sequence

Python beginners example: sum of arithmetic sequence

```python

class ArithmeticSequence():
	def __init__ (self, seq):
		self.seq = seq 
		
	def sum(self):
		summed = len(self.seq) / 2 * (self.seq[0] + self.seq[-1])
		return summed 

test_sub = [2,4,6,8,10,12,14,16]		
print(ArithmeticSequence(test_sub).sum())		
print(sum(test_sub))


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
- Another Python site: https://pythonprogramminglanguage.com
