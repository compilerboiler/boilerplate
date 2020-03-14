---
tags: ["python"]
date: 2020-02-14
title: python string substitute
---
In <a href="https://python.org">Python</a> you can easily substitute a <a href="https://pythonbasics.org/strings/">string</a> without having to do character by character replacement (looking at you <a href="https://stackoverflow.com/questions/779875/what-is-the-function-to-replace-string-in-c">C programming</a>).

In fact, Python has a method named **.replace()** which is part of the <a href="https://pythonbasics.org/strings/">string</a>.

The syntax for the replace method is:

```python
str.replace(old, new[, max])
```

Where the parameters are:

* **old** the string to be replaced
* **new** the new string
* **max** optional, maximum number of replacements

## Replace example

Take a look at this example in the Python shell.

```python
>>> s = "All work and no play makes jack a dull boy"
>>> s = s.replace("jack","Josephine")
>>> s = s.replace("boy","girl")
>>> s
'All work and no play makes Josephine a dull girl'
>>>
```

So strings get replaced and the method can be called multiple times on the same string.

By default it replaces each string it finds, with no limitation.
The following example shows the usage of replace() method.

```python
>>> x = "for philip python programming is pragmatic and powerful"
>>> x = x.replace("p","P")
>>> x
'for PhiliP Python Programming is Pragmatic and Powerful'
>>> 
```

But if you add the optional max parameter, you can limit the number of occurrences:

```python
>>> x = "for philip python programming is pragmatic and powerful"
>>> x = x.replace("p","P",1)
>>> x
'for Philip python programming is pragmatic and powerful'
>>> 
```

This also works on <a href="https://www.python.org/dev/peps/pep-0498/">f-Strings</a> (formatted-strings).

```python
>>> a = 1
>>> b = 2
>>> x = f"a is {a} and b is {b}"
>>> x = x.replace("a ","A ")
>>> x
'A is 1 and b is 2'
>>> x = x.replace("b ","B ")
>>> b
2
>>> x
'A is 1 and B is 2'
>>>
```


**Related links:**
* <a href="https://pythonbasics.org/replace/">Replace function</a>
* <a href="https://docs.python.org/3.8/library/string.html">Documentation on strings</a>
* <a href="https://pythonbasics.org/">Learn Python</a>

