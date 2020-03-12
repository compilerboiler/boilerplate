---
title: python code python-code-find-gcd (snippet)
date: 2019-02-15
tags: ["python"]
---
Python example 'python code python-code-find-gcd'

Functions in program: 
* `def gcd(numbers):`

Modules used in program: 
* `import math`

## python code python-code-find-gcd

Python code example: python code python-code-find-gcd

```python
# Find gcd of a list of numbers

from functools import reduce
import math
def gcd(numbers):
    return reduce(math.gcd, numbers)
gcd([24,108,90])


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org

More Python: https://pythonprogramminglanguage.com
