---
tags: ["python"]
date: 2020-02-14
title: python in operator
---
In the <a href="https://python.org">Python</a> programming language, the *in* operator is membership test operator. You can use it to check if a value exists in an object. 

That means you don't need to use a for loop to go through the members and use an if to compare (as you may be used to in C)

So instead of this:

```python
>>> myList = [5,7,8,11,15,17,18,22,26,28,32]
>>> for i in myList:
...     if i == 15:
...         print("found")
... 
found
>>>
```

You can do this:

```python
>>> myList = [5,7,8,11,15,17,18,22,26,28,32]
>>> if 15 in myList:
...     print("found")
... 
found
>>> 
```

The **in** operator can be used on different types of variables like <a href="https://pythonbasics.org/strings/">strings</a>, <a href="https://pythonbasics.org/list/">lists</a>, <a href="https://pythonbasics.org/dictionary/">dict</a>, files and more.

## In operator

You can see some examples below. The in operator is used to test if its part of the members.

Find if a sub-string is inside a string (is a member) with the in operator:

```python
>>> s = "hello world"
>>> if "world" in s:
...     print("found")
... 
found
>>>
```

You can use the in-keyword to find characters (strings of size 1)

```python
>>> s = "hello world"
>>> if "e" in s:
...     print("found 'e'")
... 
found 'e'
>>> 
```

### Lists

A list can be a collection of numbers, strings or other types of data. 

The in operator works on all lists, regardless of which data is inside it. You can find a number inside a list with the in operator:

```python
>>> x = [6,2,7,8,3]
>>> if 2 in x:
...     print('found')
... 
found
>>>
```

If a list contains strings instead of numbers, no problem, it can find the string.

```python
>>> x = ["Alice","Charlois","Eduard","George","Henry"]
>>> if "Eduard" in x:
...     print("Found Eduard")
... 
Found Eduard
>>>
```

### Dict

A dictionary is a key-value mapping, this is sometimes named associated array in other programming languages. A dictionary is a bit different.

For a dictionary, the in keyword finds the keys

```python
>>> x = { 'developer':'dev', 'coffee':'cof' }
>>> if 'developer' in x:
...     print("found")
... 
found
>>>
```

But not for the values in a dict:

```python
>>> x = { 'developer':'dev', 'coffee':'cof' }
>>> if 'dev' in x:
...     print("found")
>>>
```

**Related links:**
* <a href="https://python-reference.readthedocs.io/en/latest/docs/operators/in.html">In operator reference</a>
* <a href="https://pythonbasics.org">Learn Python</a>
