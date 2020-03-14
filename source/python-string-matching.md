---
tags: ["python"]
date: 2020-02-16
title: python string matching
---
---
tags: ["python"]
date: 2020-02-14
title: python string matching
---
In [Python](https://python.org) programming, if you have a string you can do comparison or so called *string matching*.

Matches the beginning or end of the [string](https://pythonbasics.org/strings/) is generally used in the matching file type or url

## Simple text matching

A simple matching function is the general `startwith()` function.

```python
>>> a = 'http://www.python.org'
>>> a.startswith ( 'http')
True
```

Note: This parameters which can be string, can also be a [tuple](https://pythonprogramminglanguage.com/tuples/). The example below passes a tuple as argument with two values.

```python
>>> a = 'http://www.python.org'
>>> a.startswith (( 'http', 'ftp'))
True
```

As you may have guessed, you can also use the method `endswith()`, with a string or tuple.

```python
>>> a = 'https://python.org'
>>> a.endswith(( '.org','.com' ))
True
>>> 
```

While tuples are similar to lists, lists are not allowed as parameter.

The parameter can not be [lists](https://pythonbasics.org/list/) or [dictionary](https://pythonprogramminglanguage.com/dictionary). If you try a list or dictionary, then you get an error

```python
>>> a = 'http://www.python.org'
>>> a.startswith ([ 'http', 'ftp'])
Traceback (most recent call last):
File "", line 1, in
a.startswith ([ 'http', 'ftp'])
TypeError: startswith first arg must be str or a tuple of str, not list
>>>
```

In fact, in addition to the above method, you can also use slices to achieve matching, but the code looks not so good:

```python
>>> a = 'https://www.python.org'
>>> a[0:4] == 'https'
True
>>>
```

## Regular expressions

Of course, we can also use [regular expressions](https://docs.python.org/3.8/howto/regex.html) to do this, but on top of it a little difficult to understand a little.

```python
>>> import re
>>> url = 'http://www.python.org'
>>> re.match ( 'http: | https: | ftp:', url)
0, 5), match = 'http:'>
>>> help (re.match)
Help on function match in module re:
      
match (pattern, string, flags = 0)
Try to apply the pattern at the start of the string, returning
a match object, or None if no match was found.
 
>>>
```

