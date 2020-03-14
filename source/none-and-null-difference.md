---
tags: ["python"]
date: 2020-02-16
title: none and null difference
---
---
tags: ["python"]
date: 2020-02-14
title: none and null difference
---
The keywords *Null* and *None*. If you are new to programming you may think they mean zero, they do not. On first sight they look alike, so what's the difference?

In many programming languages (C, Java, SQL, JavaScript) there is a Null value. Sometimes explicitly spelled as NULL or null. 

Not so in <a href="https://python.org">Python</a>, Python does not have a null value.

```python
>>> x = null
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'null' is not defined
>>> 
```

## None type

Instead there is the None object. None effectively means there is no value or it is empty. Basically, NoneType is a data type just like int, float, etc.

You can see a type using

```python
    >>> print(type(int))
    <class 'type'>
    >>> print(type(float))
    <class 'type'>
```

You can see this for the None type too:

```python
    >>> print(type(None))
    <class 'NoneType'>
```

## Assign None value

You can see above is an <a href="https://pythonbasics.org/class/">object (class)</a>, in Python this None object never has any functionality. Lets define a variable with the None value

```python
    twelve = None
    print(twelve is None)
```

See the result

```python
    >>> twelve = None
    >>> print(twelve is None)
    True
    >>> 
```

None means no value, not zero.

```python
    >>> print(twelve == 0)
    False
```

## None and null difference

Although there is no null value in Python, you can use None like null. 

```python
    >>> x = None
    >>> if x is None:
    ...     print('x is null')
    ... else:
    ...     print('x is not null')
    ... 
    x is null
```

## Redefine None

Can you redefine None to be something? No, you can't do this.

```python
    >>> None = 1
      File "<stdin>", line 1
    SyntaxError: can't assign to keyword
```

Rest assured, the value of None is always empty.


**Related links:**
* <a href="https://docs.python.org/3.8/library/constants.html?highlight=none#None">Python docs None reference</a>
* <a href="https://pythonbasics.org">Learn Python</a>


