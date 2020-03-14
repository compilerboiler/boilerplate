---
date: 2020-02-16
title: remove trailing spaces python
---
If you have a Python text [string](https://pythonbasics.org/strings/), and want trailing spaces removed you can do that with the method `.strip()`, `.lstrip()` and `.rstrip()`.

That removes the spaces before and after the string.

# Example

You can use strip, lstrip, rstrip methods. Like the name suggests, `lstrip` strips left of the string, `rstrip` strips right of the string and `strip` just strips the string of spaces.

First create a string surrounded by spaces:

```python
>>> a = "abc".center(30)
>>> a
'             abc              '
>>>
```

To do a left strip, call the method `lstrip()`. This removes spaces to the left of the string:

```python
>>> b = a.lstrip()
>>> b
'abc              '
```

The results of a right strip, call `rstrip()` which removes spaces to the right of the string:

```python
>>> 
>>> c = a.rstrip()
>>> c
'             abc'
```

To do a general strip, that removes all spaces on both sides:

```python
>>> 
>>> d = a.strip()
>>> d
'abc'
>>> 
>>> 
```

The `strip()` function only does trailing spaces, not spaces inside the string itself.

```python
>>> a = "    aaaa  bbbb ccc    dddd   eee           "
>>> a.strip()
'aaaa  bbbb ccc    dddd   eee'
>>> 
```

