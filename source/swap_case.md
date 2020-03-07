---
title: swap case (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'swap case'

Functions in program: 
* `def swap_case(s):`

## swap case

Python beginners example: swap case

```python
def swap_case(s):
    swapped = ""
    for i in range(len(s)):
        temp = s[i].upper()
        if (s[i] == temp):
            swapped += s[i].lower()
        else:
            swapped += s[i].upper()
            
    return swapped    


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
