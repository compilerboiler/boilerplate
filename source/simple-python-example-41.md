---
title: simple python-example-41 (snippet)
date: 2020-02-10
tags: ["python"]
---
Python example 'python-example-41'

Functions in program: 
* `def varfunc():`

## python-example-41

Python example: python-example-41

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

def varfunc():
    var = 0
    print('var = %d' % var)
    var += 1
if __name__ == '__main__':
    for i in range(3):
        varfunc()

# 类的属性
# 作为类的一个属性吧
class Static:
    StaticVar = 5
    def varfunc(self):
        self.StaticVar += 1
        print(self.StaticVar)

print(Static.StaticVar)
a = Static()
for i in range(3):
    a.varfunc()


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
