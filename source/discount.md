---
title: discount (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'discount'

Functions in program: 
* `def percToDiscount(percent , mp):`

## discount

Python beginners example: discount

```python
def percToDiscount(percent , mp):
    discount = percent / 100 * mp
    return('Discount is : ' + str(discount))

print('Hello\n')
print('Press Enter to exit')
while(True):  # I've put counting discount in a loop cause if you want to count on multiple items
    more = str(input('Count or End : '))
    if more == 'Count':
        disCountPerc = float(input('Discount Percent : '))
        marketPrice = float(input('Market Price : '))
        print(percToDiscount(disCountPerc , marketPrice))
        continue
    else:
        quit()


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
