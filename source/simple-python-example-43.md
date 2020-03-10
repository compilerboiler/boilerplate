---
title: simple python-example-43 (snippet)
date: 2020-02-11
tags: ["python"]
---
Python example 'python-example-43'


## python-example-43

Python example: python-example-43

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

class Num:
    nNum = 1
    def inc(self):
        self.nNum += 1
        print('nNum = %d' % self.nNum)

if __name__ == '__main__':
    nNum = 2
    inst = Num()
    for i in range(3):
        nNum += 1
        print('The num = %d' % nNum)
        inst.inc()


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
