---
title: simple python-example-79 (snippet)
date: 2020-02-11
tags: ["python"]
---
Python example 'python-example-79'


## python-example-79

Python example: python-example-79

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

if __name__ == '__main__':
    str1 = raw_input('input string:\n')
    str2 = raw_input('input string:\n')
    str3 = raw_input('input string:\n')
    print(str1,str2,str3)
    
    if str1 > str2 : str1,str2 = str2,str1
    if str1 > str3 : str1,str3 = str3,str1
    if str2 > str3 : str2,str3 = str3,str2

    print('after being sorted.')
    print(str1,str2,str3)


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
