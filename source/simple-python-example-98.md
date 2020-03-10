---
title: simple python-example-98 (snippet)
date: 2020-02-10
tags: ["python"]
---
Python example 'python-example-98'


## python-example-98

Python example: python-example-98

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

if __name__ == '__main__':
    fp = open('test.txt','w')
    string = raw_input('please input a string:\n')
    string = string.upper()
    fp.write(string)
    fp = open('test.txt','r')
    print(fp.read())
    fp.close()


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
