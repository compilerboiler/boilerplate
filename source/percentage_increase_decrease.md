---
title: percentage increase decrease (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'percentage increase decrease'

Functions in program: 
* `def decreasePercent(decrease , origValue):`
* `def increasePercent(increase , origValue):`

## percentage increase decrease

Python beginners example: percentage increase decrease

```python
# Percantage Increase , Percentage Decrease

def increasePercent(increase , origValue):
    return(str(increase / origValue * 100) + '%')

def decreasePercent(decrease , origValue):
    return(str(decrease / origValue * 100) + '%')

print('Hello,\nPress Enter To Exit')
incOrDec = str(input('increase or decrease: ')).strip().lower()
if incOrDec == 'increase':
    print(increasePercent(float(input('Increased Value : ')) ,  float(input('Orignal Value : '))))
elif incOrDec == 'decrease':
    print(increasePercent(float(input('Increased Value : ')), float(input('Orignal Value : '))))
else:
    quit()


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
