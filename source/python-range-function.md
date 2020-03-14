---
tags: ["python"]
date: 2020-02-14
title: python range function
---
<a href="https://python.org">Python</a> has a function that generates numbers, the *range* function. This function creates a list of numbers.

The range function is often used in a <a href="https://pythonbasics.org/for-loops/">for loop</a>, to repeat a certain number of times. You can see it used for creating a list of numbers too, writing down every number manually is just to cumbersome.


## Range list examples

If the range function has only one parameter, it will count from zero to the end.

    range(end)

In Python 3 you must parse it to a list. Thus making it a simple numeric list. We store the list in variable l, which we then use to output.

    >>> l = list(range(5))
    >>> print(l)
    [0, 1, 2, 3, 4]
    >>> 


The function permits definition of starting and step size. To start at 5 and have a step size of 2:

    >>> l = list(range(5,50,2))
    >>> print(l)
    [5, 7, 9, 11, 13, 15, 17, 19, 21, 23, 25, 27, 29, 31, 33, 35, 37, 39, 41, 43, 45, 47, 49]
    >>> 

<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fthumbs.gfycat.com%2FAchingWellinformedIndianrhinoceros-max-1mb.gif&f=1&nofb=1"> 

## Range loop example

For loops are one way of repeating code (iteration). That means, you don't have to rewrite the same instructions over and over but just can "jump back" or repeat lines.

For use in a for loop you don't need to parse to a list,

    >>> for i in range(0,6):
    ...     print(i)
    ... 
    0
    1
    2
    3
    4
    5
    >>> 

In the for loop you can use step size and starting value. In this case starting at 1 with a step size of 3.

    >>> for i in range(1,30,3):
    ...     print(i)
    ... 
    1
    4
    7
    10
    13
    16
    19
    22
    25
    28
    >>>

**Related links:**
* <a href="https://docs.python.org/3.5/library/stdtypes.html#typesseq-range">Range function in Python docs</a>
* <a href="https://pythonbasics.org">Learn Python programming</a>
* <a href="https://gum.co/dcsp">Python course</a>


