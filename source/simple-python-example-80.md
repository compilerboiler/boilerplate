---
title: simple python-example-80 (snippet)
date: 2020-02-11
tags: ["python"]
---
Python example 'python-example-80'


## python-example-80

Python example: python-example-80

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

if __name__ == '__main__':
    i = 0
    j = 1
    x = 0
    while (i < 5) :
        x = 4 * j
        for i in range(0,5) :
            if(x%4 != 0) :
                break
            else :
                i += 1
            x = (x/4) * 5 +1
        j += 1
    print(x)


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
