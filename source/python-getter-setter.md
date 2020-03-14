---
date: 2020-02-16
title: python getter setter
---
---
tags: ["python"]
date: 2020-02-16
title: python getter setter
---
---
tags: ["python"]
date: 2020-02-14
title: python getter setter
---
The [Python](https://python.org) `setattr()` function corresponds to the function `getattr()`. It set the attribute values of an object.

Python is an object orientated language, so you can have multiple objects in your applications run-time. 

Objects (from [classes](https://pythonbasics.org/class/)) can have unique values. These values should be set using a getter and setter function. Python has the functions `setattr()` and `getattr()` for that.

The setattr() syntax is:
```python
setattr (object, name, value)
```
with parameters:

* Object: the object.
* Name: string, object properties.
* Value: property value.

### examples

The following examples illustrate `setattr()` function using the method:

```python
>>> class A:
...    foo = 1
... 
>>> obj1 = A()
>>> getattr(obj1, 'foo')
1
>>> setattr(obj1, 'foo', 6)
>>> getattr(obj1, 'foo')
6
>>> 
```

Of course you can use properties without getter and setter, but that's a bad practice.

```python
>>> obj1.foo
6
>>> obj1.foo = 7
>>> 
```

If the property does not exist will create a new object property, and it will do property assignment:

```python
>>> obj1.name = "Alice"
>>> getattr(obj1, 'name')
'Alice'
>>> 
```

This modifies the existing object only, not the class the object is derived from.

```python
>>> dir(A)
['__class__', '__delattr__', '__dict__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__gt__', '__hash__', '__init__', '__init_subclass__', '__le__', '__lt__', '__module__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__setattr__', '__sizeof__', '__str__', '__subclasshook__', '__weakref__', 'foo']
>>> 
```

But you should define all properties in the class, this is a best practice.

**Related links:**
* [Python programming book](https://gumroad.com/l/dcsp)
* [Setattr Python docs reference](https://docs.python.org/3.5/library/functions.html#setattr)
