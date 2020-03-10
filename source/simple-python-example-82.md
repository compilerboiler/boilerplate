---
title: simple python-example-82 (snippet)
date: 2020-02-10
tags: ["python"]
---
Python example 'python-example-82'


## python-example-82

Python example: python-example-82

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

if __name__ == '__main__':
    n = 0
    p = raw_input('input a octal number:\n')
    for i in range(len(p)):
        n = n * 8 + ord(p[i]) - ord('0')
    print(n)


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
