---
title: distance on number line (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'distance on number line'

Functions in program: 
* `def distance(x,y):`

## distance on number line

Python beginners example: distance on number line

```python
# this is a simple geometric distance formula
# d(x,y) = |x-y| = distance
# where x and y are co-ordinates on a number line

def distance(x,y):
   return abs(x-y)

flag = True
while flag:
    usr = str(input("start [Y/n]: ")).strip().lower()
    if usr == "y":
        print(distance(float(input("Value of X co-ordinate: ")), float(input("Value of Y co-ordinate: ")) ), "\n")
    else:
        flag = False


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
