---
title: discountPercent (snippet)
date: 2019-02-07
tags: ["python"]
---

## discountPercent

Python beginners example: discountPercent

```python
def iLoveDiscount(discount , mp):  # mp is market price
    discountPerc = discount / mp * 100
    return('Discount is ' + str(discountPerc) + '%')

print('Hello\n')
print('Press Enter to exit')
while(True):  # I've put counting discount in a loop cause if you want to count on multiple items
    more = str(input('Count or End : '))
    if more == 'Count':
        disCount = float(input('Discount : '))
        marketPrice = float(input('Market Price : '))
        print(iLoveDiscount(disCount , marketPrice))
        continue
    else:
        quit()


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
