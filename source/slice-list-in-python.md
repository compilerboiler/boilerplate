---
date: 2020-02-16
title: slice list in python
---
---
tags: ["python"]
date: 2020-02-16
title: slice list in python
---
---
tags: ["python"]
date: 2020-02-14
title: slice list in python
---
The <a href="https://python.org">Python</a> programming language has support for lists, a <a href="https://pythonspot.com/python-lists/">list</a> is a collection. It can be a collection of numbers, strings or other types of data.

The example below defines the list x:

```python
x = [ 1,2,3,4,5,6,7,8 ]
```
How do you get only a part of the list?
You may think a <a href="https://pythonbasics.org/for-loops/">for loop</a>, which does the job, but there's an easier way.

## Slice list

The Pythonic way is by defining brackets with start and ending position.
In between you write a colon, not a comma. Like this:

```python
>>> x[1:3]
```

This looks similar to defining a list, but instead it takes a slice of the list.

This starts at the 2nd position (the element in Python is zero), and ends at the 4th position (3rd counting from zero). This may be a bit confusing initially.

```python
>>> x = [1,2,3,4,5,6,7,8]
>>> x[1:3]
[2, 3]
>>> x[0:2]
[1, 2]
>>> x[0:3]
[1, 2, 3]
>>> 
```

If you want to start from the first character, you can leave the starting number out:

```python
>>> x[:2]
[1, 2]
>>> x[:3]
[1, 2, 3]
>>> 
```

To create a new list, you can just do this:

```python
>>> z = x[:2]
>>> z
[1, 2]
>>> 
```

You can use a list as an object, it supports function calls. This lets you sort the list, remove elements and more.

**Related links:**
* <a href="https://docs.python.org/3.8/tutorial/datastructures.html">List in Python docs</a>
* <a href="https://pythonbasics.org">Learn Python</a>


