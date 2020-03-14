---
date: 2020-02-16
title: python why enummerate
---
This post will discuss the <a href="https://python.org">Python</a> <a href="https://pythonbasics.org/enumerate/">enumerate</a> function quickly. Python is known to make code readable and using enumerate will make your code more readable. 

## Simple loops

Loops let you repeat lines of code, the most common being for loops and while loop. If you have previous experience with <a href="https://pythonprogramminglanguage.com/for-loops/">for loops</a>, you may be inclined to use an index (i) on the array.

```python
>>> array = ['a','b','c','d','e']
>>> for i in range(len(array)):
...     print(array[i])
... 
a
b
c
d
e
>>> 
```

If you have been programming during the C++ days, you may even be inclined to do something like this:

```python
>>> i = 0
>>> while i < len(array):
...     print(array[i])
...     i = i + 1
```

This is overcomplicated. Python is mucher easier

## How to use enumerate

This works, but it's not Pythonic. Instead `enumerate` makes this more readable (It's also easier to code).

The enumerate function takes an iterable (<a href="https://pythonbasics.org/list/">array</a>) and for each element gives the value and index.

```python
>>> array = ['a','b','c','d','e']
>>> for index, item in enumerate(array):
...     print(item)
... 
a
b
c
d
e
>>> 
```

Much better! You get the index as well as the element, without having to keep track of the index variable.

The `enumerate` function works on arrays (lists) or other types of sequences like tuples, strings etc.

```python
>>> array = [ 1,3,2,6,3,9,4,12,5,15,6,18,7,21,8 ]
>>> for index, item in enumerate(array):
...     print(item)
... 
```

So `enumerate` is a very useful function that makes programming a bit simpler.



