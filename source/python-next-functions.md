---
date: 2020-02-16
title: python next functions
---
---
tags: ["python"]
date: 2020-02-16
title: python next functions
---
---
tags: ["python"]
date: 2020-02-14
title: python next functions
---
In this article we'll discuss the [Python](https://python.org) `next()` function. The Python next() function returns an iterator to the next item. If you have an iterable, it makes sense to use the next() function.

The next() syntax is:

```python
next (iterator [, default])
```
Where the parameters are:

* Iterator: [iterables](https://pythonbasics.org/iterable/)
* Default: optional, used to set the default return value when there is no next element, if not set, and no next element is found it triggers the StopIteration exception.

The function return the current object in the iteratable.

### examples

The following example shows how to use the next of:

```python
#!/usr/bin/python
#-*- coding: UTF-8 -*-

# First get Iterator object:
it = iter ([1, 2, 3, 4, 5])

# Cycle:
while True:
    try:
        # Get the next value:
        x = next(it)
        print(x)
    except StopIteration:
        # Encounter StopIteration loop exits
        break
```

The output is:

```
    1
    2
    3
    4
    5
```

It raises a `StopIteration` exception that you must catch, because otherwise the program stops abruptly (an exception is an 'error' that occurs while the program is running).

```python
>>> 
>>> nums = [1,2,3,4,5,6]
>>> it = iter(nums)
>>> while True:
...     x = next(it)
...     print(x)
... 
1
2
3
4
5
6
Traceback (most recent call last):
  File "<stdin>", line 2, in <module>
StopIteration
>>> 
```

So catch the `StopIteration` exception with a [try-except](https://pythonbasics.org/try-except/) block.

```python
>>> nums = [1,2,3,4,5,6]
>>> it = iter(nums)
>>> while True:
...     try:
...         x = next(it)
...         print(x)
...     except StopIteration:
...         break
... 
```

**Related links:**
* [Learn Python programming](https://gumroad.com/l/dcsp)
* [Python docs next() reference](https://docs.python.org/3.5/library/functions.html#next)

