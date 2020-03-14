---
tags: ["python"]
date: 2020-02-14
title: pass statements
---
In some programming languages there are is a statement that does nothing. In assembly there's `nop` (no operation). How about Python?

In Python you can use the `pass` statement. The `pass` statement does nothing.

## Why pass?

Python has the syntactical requirement that code blocks (for, if, except, def, class etc.) are not empty. 

Empty code blocks are useful in different contexts, such as when you don't have time to implement right now. 

```python
def complexFunction():
    pass
```

Other purposes are deriving an exception class that does not add new behaviour

```python
class CustomException(Exception):
    pass
```

if you want to ignore a type of Exception

```python
try:
    self.version = "Expat %d.%d.%d" % expat.version_info
except:
    pass # unknown
```

Below are some more pass examples

## Pass examples

If nothing is supposed to happen in a code block, a pass is needed for such a block to not produce an IndentationError


You can use this for all kinds of purposes. Inside a while loop:

```python
>>> while True:
...     pass 
```

This will wait for a keyboard interrupt (Ctrl+C)

In a <a href="https://pythonbasics.org/class/">class</a> that you need to implement, but will implement later:


```python
>>> class Example:
...     pass
...
```

But beware, if a class is not implemented you can still create objects:

```python
>>> obj = Example()
>>> 
```

In a function that you implement later:

```python
>>> def hello():
...     pass   # Implement this later
```

**Related links:**
* <a href="https://pythonbasics.org">Learn Python Programming</a>
* <a href="https://medium.com/better-programming/how-to-use-pass-break-and-continue-in-python-6e0201fc032a">How to use pass, break and continue</a>
