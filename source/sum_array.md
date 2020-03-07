---
title: sum array (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'sum array'

Functions in program: 
* def sum_arr(n):

## sum array

Python beginners example: sum array

```python
def sum_arr(n):
    res = 0
    for x in n:
        res += x
    return res

nums = [52345,746587,98589,54398,9348,45887,49856]
test = sum_arr(nums)
if test == sum(nums):
    print("Sum of arr: {}".format(test))
else:
    print("Func dosen't work!")
# Most simple algorithm ever! Isn't it!


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
- Another Python site: https://pythonprogramminglanguage.com
