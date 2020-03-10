---
title: simple python-example-17 (snippet)
date: 2020-02-11
tags: ["python"]
---
Python example 'python-example-17'


Modules used in program: 
* `import string`

## python-example-17

Python example: python-example-17

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

import string
s = raw_input('input a string:\n')
letters = 0
space = 0
digit = 0
others = 0
for c in s:
    if c.isalpha():
        letters += 1
    elif c.isspace():
        space += 1
    elif c.isdigit():
        digit += 1
    else:
        others += 1
print('char = %d,space = %d,digit = %d,others = %d' % (letters,space,digit,others))


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
