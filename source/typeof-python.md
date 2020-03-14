---
tags: ["python"]
date: 2020-02-14
title: typeof python
---
In <a href="https://python.org">Python</a>, everything is an object (from <a href="https://pythonspot.com/objects-and-classes/">object orientated programming</a>). This is very different from other programming languages like C++, where object oriented programming is more of an addition to the functional language.

Python is not a functional language, it is highly object orientated. In Python, every object is derived from a <a href="https://pythonbasics.org/class/">class</a>. 

Many programming languages support some type of object orientated programming. For example, you could have some objects that are created from the class car (in C# code):

![class and objects](https://dev-to-uploads.s3.amazonaws.com/i/kj8370lwsrd8lxpitamg.png)

To get the type of an object, you can use the type() function. This returns the class the object is created from.

The type of object can be requested in the Python shell (sometimes named <a href="https://pythonprogramminglanguage.com/repl/">REPL</a>).

As parameter pass the object, it returns the type of the object.

## Examples

The examples below run from the Python interactive shell.
Lets try that:

```python
>>> type({})
<class 'dict'>
```

what about a list?

```python
>>> type([])
<class 'list'>
>>> 
```

What if we create a list, store it in a variable and request the type?

```python
>>> x = [1,2,3,4]
>>> type(x)
<class 'list'>
>>> 
```

Above shows that works too. If you change x to be a dict, it will tell you that.

```python
>>> x = { 'a':1, 'b':2 }
>>> type(x)
<class 'dict'>
>>
```

What about text?

```python
>>> x = "hello world"
>>> type(x)
<class 'str'>
```

Yes, that's a string.
How about numbers?


```python
>>> x = 3
>>> type(x)
<class 'int'>
```

```python
>>> x = 3.0
>>> type(x)
<class 'float'>
>>>
```

So you can get the type for any object. 

**Related links:**
* <a href="https://python.org">Python Official Site</a>
* <a href="https://pythonbasics.org/">Learn Python</a>
