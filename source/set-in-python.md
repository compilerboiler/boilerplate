---
tags: ["python"]
date: 2020-02-16
title: set in python
---
---
tags: ["python"]
date: 2020-02-14
title: set in python
---
In <a href="https://python.org">Python</a>, a `set` is a container whose objects must be unique. If you try to add something that's already in the set, it will not do anything (no error will be thrown).

## Set example

Open the Python <a href="https://pythonprogramminglanguage.com/repl/">interactive shell</a> to try it out. You can define a set by calling the *set()* method.

```python
    >>> a = set([1,1,1,1,2,2,2,2,3,3,3,3,3,3,4,4,4])
    >>> a
    {1, 2, 3, 4}
    >>> 
```

It uses curly braces `{` `}`, but don't be confused with a <a href="https://pythonprogramminglanguage.com/dictionary/">dictionary</a> because it's a set. You can double check this with the type() function

```python
    >>> type(a)
    <class 'set'>
    >>> 
```

To add elements to the set, use the `.add(object)` method.

```python
    >>> a.add(4)
    >>> a.add(5)
    >>> a.add(6)
    >>> a
    {1, 2, 3, 4, 5, 6}
    >>> 
```

You can remove elements with the pop() method

```python
    >>> a
    {2, 3, 4, 5, 6}
    >>> a.pop()
    2
    >>> a
    {3, 4, 5, 6}
    >>> 
```

To remove a specific item call the `.remove()` method

```python
    >>> a.remove(5)
    >>> a    
    {3, 4, 6}
    >>> 
```

## FrozenSet

A <a href="https://docs.python.org/2.4/lib/types-set.html">frozenset</a> is different in mutability: it's frozen, cannot be changed, modified.

You can try adding or removing elements in the Python interactive shell:

```python
>>> a = frozenset([1,1,1,1,2,2,2,2,3,3,3,3,3,3,4,4,4])
>>> a
frozenset({1, 2, 3, 4})
>>> a.add(5)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
AttributeError: 'frozenset' object has no attribute 'add'
>>> 
```

## Operations on sets

You can do a variety of operations on sets

```python
>>> pets = { 'cat','parrot','dog' }
>>> zoo = { 'elephant','rhino','dog' }
```

Intersection of two sets

```python
>>> pets & zoo
{'dog'}
```

Union of two sets

```python
>>> pets | zoo
{'dog', 'parrot', 'elephant', 'rhino', 'cat'}
```

Symmetric difference of two sets

```python
>>> pets ^ zoo
{'parrot', 'elephant', 'rhino', 'cat'}
```

Asymmetric difference of two sets

```python
>>> pets - zoo
{'cat', 'parrot'}
>>> 
```

You can test if a set contains an object, by using the `in` keyword. This returns a <a href="https://pythonprogramminglanguage.com/booleans/">boolean</a> value (**True**/**False**). 

```python
>>> 'cat' in pets
True
>>> 'rhino' in pets
False
>>> 
```

The `in` keyword can also be applied to other sequences like <a href="https://stackoverflow.com/questions/626759/whats-the-difference-between-lists-and-tuples">tuples</a> or <a href="https://pythonbasics.org/list/">lists</a>.

The typical operations you'd expect like `min(set)`, `max(set)` and `len(set)` can be applied too.



