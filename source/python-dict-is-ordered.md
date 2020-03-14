---
date: 2020-02-16
title: python dict is ordered
---
---
tags: ["python"]
date: 2020-02-16
title: python dict is ordered
---
---
tags: ["python"]
date: 2020-02-14
title: python dict is ordered
---
In <a href="https://python.org">Python</a>, a <a href="https://pythonbasics.org/dictionary/">dictionary</a> is Pythons version of a map (associative array or hash table). It lets you map keys to values. This makes it easy to request a value given a key.

A hash table contains both keys and values, but they are in a pseudo random order. This is different from a list (array), that only contains elements.

![array vs map](https://dev-to-uploads.s3.amazonaws.com/i/ape4n1prp6eyore5bgia.png)

*the good news: a dict in Python is now in insertion order*

## Dicts are ordered (for newest Python version)

In the newest version of Python, a dictionary is now in insertion order. That has not always been the case.

```python
➜  ~ python3.7
Python 3.7.5 (default, Nov 20 2019, 09:21:52) 
[GCC 9.2.1 20191008] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>
>>> d = {'one': True, 'two': True, 'three': True, 'four': True, 'five': True}
>>> d['two']
True
>>> d['four']
True
>>> d
{'one': True, 'two': True, 'three': True, 'four': True, 'five': True}
>>> 
```

If you used an older version of Python, there was no guarantee that the dictionary is in order.

For example, in the older version of Python (2.x)

```python
~ python2
Python 2.7.17 (default, Nov  7 2019, 10:07:09) 
[GCC 9.2.1 20191008] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> d = {'one': True, 'two': True, 'three': True, 'four': True, 'five': True}
>>> d
{'four': True, 'three': True, 'five': True, 'two': True, 'one': True}
>>>
```

Quoting the docs referenced above:

    Changed in version 3.7: Dictionary order is guaranteed to be insertion 
    order. This behavior was an implementation detail of CPython from 3.6.

**Related links:**
* <a href="https://pythonprogramminglanguage.com/dictionary/">Dictionaries in Python</a>
* <a href="https://gumroad.com/l/dcsp">Python programming course</a>

