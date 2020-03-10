---
title: simple python-example-3 (snippet)
date: 2020-02-10
tags: ["python"]
---
Python example 'python-example-3'


Modules used in program: 
* `import math`

## python-example-3

Python example: python-example-3

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

import math
for i in range(10000):
    #转化为整型值
    x = int(math.sqrt(i + 100))
    y = int(math.sqrt(i + 268))
    if(x * x == i + 100) and (y * y == i + 268):
        print(i)


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
