---
date: 2020-02-16
title: string contains python
---
In the <a href="https://python.org">Python</a> programming language, you can work with strings. A <a href="https://pythonbasics.org/strings/">string</a> is a text object in Python. If you have a large string (sentence, paragraph, chapter, book), you may want to search in it.

Searching in a large string, is known as finding a sub-string. Programming languages handle with this in different ways.

How to find a sub-string in Python?

If you programmed in other languages before, you may know string.contains() or string.indexof()

```c
if not string.contains("word"):
   continue
```

## Examples

Python doesn't have these, but it's not hard to find sub-strings. You can use the *in* keyword like this:

```python
    >>> s = "Hello World"
    >>> if "World" in s:
    ...     print("found")
    ... 
    found
    >>> 
```

You can use the string method .find() too

```python
>>> if s.find("World") != -1:
...     print("Found")
... 
Found
>>>
```

## Case sensitive

Both are case-sensitive, so this won't return anything because the first capital letter is missing:

```python
>>> if s.find("world") != -1:
...     print("Found")
... 
```

To avoid case-sensitive problems, you can call the lower() method on both strings.

```python
>>> if "World".lower() in s.lower():
...     print("Found")
... 
Found
```

This works for different characters too, but be careful with non-English characters. Like the Portugese word for read ("lê")

```python
>>> s = "lê"
>>> if "LÊ".lower() in s.lower():
...     print("Found")
... 
Found
```

But only for newest versions of Python! If you try the same in an older version of Python:

```python
python2
Python 2.7.17 (default, Nov  7 2019, 10:07:09) 
[GCC 9.2.1 20191008] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> s = "lê"
>>> if "LÊ".lower() in s.lower():
...     print("Found")
... 
>>
```

To prevent problems like this, you want to rely on **casefold()**.

```python
>>> s = "lê"
>>> if "LÊ".casefold() in s.casefold():
...     print("Found")
... 
Found
>>> 
```

**Related links:**
* <a href="https://pythonbasics.org/strings/">More on Python strings</a>
* <a href="https://python.org">Python official homepage</a>
* <a href="https://pythonbasics.org/">Learn Python</a>

