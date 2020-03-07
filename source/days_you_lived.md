---
title: days you lived (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'days you lived'

Functions in program: 
* `def daysBetweenDates(year1, month1, day1, year2, month2, day2):`

## days you lived

Python beginners example: days you lived

```python
# We assume that given dates are correct
# and 
# solved for problem set in cs course on udacity.com

from calendar import isleap

def daysBetweenDates(year1, month1, day1, year2, month2, day2):
    dom = [ 31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
    domleap = [ 31, 29, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
    if (isleap(year1) and isleap(year2)):
        e1 = sum(domleap) + sum(domleap[:month1 - 1]) + day1
        e2 = sum(domleap) + sum(domleap[:month2 - 1]) + day2
        return e2 - e1
    
    days = 0
    if isleap(year1):
        days += (sum(domleap[month1 - 1:]) - day1) + sum(dom[:month2 - 1]) + day2 
    elif isleap(year2):
        days += (sum(dom[month1 - 1:]) - day1) + sum(domleap[:month2 - 1]) + day2 
    else:
        days += (sum(dom[month1 - 1:]) - day1) + sum(dom[:month2 - 1]) + day2 
    for year in range(year1 + 1, year2):
        if isleap(year):
            days += sum(domleap)
        else:
            days += sum(dom)
    return days
    


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
