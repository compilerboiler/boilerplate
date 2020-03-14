---
tags: ["python"]
date: 2020-02-16
title: things you must know about python strings
---
---
tags: ["python"]
date: 2020-02-14
title: things you must know about python strings
---
[Python](https://python.org) strings let you work with text. If you define text e.g. Python string, you can do so in two ways:
```python
>>> s = 'abc'
>>> s
'abc'
>>>
>>> s = "abc"
>>> s
'abc'
>>> 
```

So single quoted [string](https://pythonbasics.org/strings/) is the same as double quoted. You can be use this interchangeably, but preferably just pick one.

You can even introduce quotes inside the strings:

```python
      >>> 'abc "d'," abc'd "
      ( 'abc "d'," abc'd ")
```

Python can automatically merge strings. To do so you should use a `+` instead of a comma. A comma will give you a tuple.

So not this:

```python
>>> s = "hello ","world"
>>> s
('hello ', 'world')
```

Also, in the above example: the comma in the middle of the string, so the final form is a tuple rather than a string

But this concatenates strings:

```python
>>> s = "hello " + "world"
>>> s
'hello world'
>>> 
```

## Use the escape character for special characters

Python supports many special characters. An escape character starts with a slash.

```python
>>> print('hello\nhello\n',end='')
hello
hello
>>> 
```

Common escape characters:

Escape | sense
--- | ---
\ | Continuous, then the top line
\ | Backslash
\'| Single quotes
\"| Double quotes
\n | Newline
\a | Bell
\b | back
\f | feed
\r | returned
\t | horizontal tab
\v | vertical tab
\n{id} | unicode database id
\Uhhhh | unicode16 bit hexadecimal value
\Uhhhh | unicode32 bit hexadecimal value
\Xhh | hexadecimal values
\Ooo | octal value
\0 | Null
