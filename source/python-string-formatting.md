---
tags: ["python"]
date: 2020-02-16
title: python string formatting
---
---
tags: ["python"]
date: 2020-02-14
title: python string formatting
---
You can do two ways of string formatting in Python. The most easy way is to use f-strings or formatted strings.  The other way is similar to the printf function in the C programming language.

The printf way:
```python
>>> print('this is %d %s pet' % (1,'hungry'))
this is 1 hungry pet
>>> 
```
The f-strings way (has an f in front of the string):
```python
>>> n = 1
>>> s = 'hungry'
>>> print(f'this is {n} {s} pet')
this is 1 hungry pet
>>> 
```
Obviously the f-strings way is better, but you may find code with the old C style way. So in the C printf way, what is this `%`?

It lets you output a type of variable. For a string `%s`, for a number `%d`.

```python
>>> 
>>> name = 'goofy'
>>> 'my name is %s ' % name
'my name is goofy '
>>> 'that will be %d dollars please' % 5
'that will be 5 dollars please'
>>> 
```

So you know `%d` and %s` string formatting codes, but there are others. 

Code | meaning
--- | ---
%s | string (or any object)
%r | s, but with repr, rather than the str
%c | character
%d | a decimal integer
%i | integer
%u | Unsigned integer
%o | octal integer
%x | hexadecimal integer
%X | x, but the print uppercase
%e | floating-point index
%E | e, but prints uppercase
%f | floating decimal
%F | floating decimal
%g | e or f floating point
%G | floating point e or f

    >>> a = 678
    >>> print('integer %i is a number' % a)
    integer 678 is a number
    >>> 

If you want a float, change it:

    >>> a = 1.23456
    >>> print('float has value of %f ' %a)
    float has value of 1.234560 
    >>> 

You can use multiple variables in a string:

    >>> name = 'goofy'
    >>> age = 50
    >>> print('I am %s and I am %d years old' % (name,age))
    I am goofy and I am 50 years old
    >>> 

Read more:
* [Python formatted strings](https://www.python.org/dev/peps/pep-0498/)
* [Python string examples](https://pythonbasics.org/strings/)

