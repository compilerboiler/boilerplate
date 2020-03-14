---
tags: ["python"]
date: 2020-02-16
title: python slice
---
---
tags: ["python"]
date: 2020-02-14
title: python slice
---
You can use the [Pythons](https://python.org) `slice()` function to create object slices. It is mainly used in the slicing operation in the function parameter. 

You can use the `slice()` function for [string slicing](https://pythonspot.com/string-slices-part-2/). The difference with default slicing `[start:stop]` is that it looks nice.
 
You can use it like `slice(stop)` or `slice(start, stop [, step])```
The parameters are: 

* Start: Starting position
* Stop: End position
* Step: spacing

The function returns an object slice.

### examples

The following example shows how to use the slice of:

    >>> myslice = slice(5)
    >>> myslice
    slice(None, 5, None)
    >>> 
    >>> a = range(10)
    >>> a
    range(0, 10)
    >>> a[myslice]
    range(0, 5)
    >>> 

You can use the `slice()` method to to create a slice of a [list](https://pythonbasics.org/list/). You can do this instead of `[2:4]`:

    >>> x = ['a','b','c','d','e']
    >>> x[slice(2,4)]
    ['c', 'd']

or a more beautiful way to write it:

    >>> x = ['a','b','c','d','e']
    >>> myslice = slice(2,4)
    >>> x[myslice]
    ['c', 'd']
    >>> 



