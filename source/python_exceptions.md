---
title: python exceptions (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'python exceptions'

Functions in program: 
* def another_method():
* def some_method():

## python exceptions

Python beginners example: python exceptions

```python
#!/usr/bin/python

class MyMethodNotImplementedError(Exception):
  def __init__(self):  
    Exception.__init__(self)

#We will raise an Error if this method is called. The purpose is to show which
#Error to use to signal that a method os not yet implemented and also to show
#how to raise Exceptions
def some_method():
  raise NotImplementedError

def another_method():
  raise MyMethodNotImplementedError()

try:
  some_method()
except NotImplementedError, e:
  print('Method is not implemented ', e)

another_method()


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
- Another Python site: https://pythonprogramminglanguage.com
