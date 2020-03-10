---
title: simple python-example-49 (snippet)
date: 2020-02-11
tags: ["python"]
---
Python example 'python-example-49'


## python-example-49

Python example: python-example-49

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

MAXIMUM = lambda x,y :  (x > y) * x + (x < y) * y
MINIMUM = lambda x,y :  (x > y) * y + (x < y) * x

if __name__ == '__main__':
    a = 10
    b = 20
    print('The largar one is %d' % MAXIMUM(a,b))
    print('The lower one is %d' % MINIMUM(a,b))


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
