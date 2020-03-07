---
title: nearest square and its root (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'nearest square and its root'

Functions in program: 
* `def nearest_square(n):`

## nearest square and its root

Python beginners example: nearest square and its root

```python
# Find the nearest root and its square

def nearest_square(n):
    i = 0
    found = False
    while (not found):
        if i ** 2 <= n < ((i + 1) ** 2):
            found = True
        else:
            i += 1
    return (i, i ** 2)
    
# Test
case = 40
res = nearest_square(case)
print("Nearest square to {}: \n{}".format(case, res[1]))


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
