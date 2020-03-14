---
tags: ["python"]
date: 2020-02-14
title: python zip function
---
In <a href="https://python.org">Python</a> you can aggregate <a href="https://pythonbasics.org/iterable/">iteratables</a> (<a href="https://pythonbasics.org/list/">lists</a>, <a href="https://pythonspot.com/python-tuples/">tuples</a>). You can do that with the zip() function, which has nothing to do with the package format zip.

Before playing with the zip function, you should know the <a href="https://pythonbasics.org">basics of Python</a>.

The zip() function takes iterables, aggregates them in a tuple, and then return it. As argument define the iteratables: *zip(iterator1, iterator2, iterator3 ...)*

You can create two lists:

```python
>>> a = [1,2,3]
>>> b = [4,5,6]
```

Then use the zip function and you'll see it aggregated both lists:

```python
>>> result = zip(a,b)
>>> result = list(result)
>>> print(result)
[(1, 4), (2, 5), (3, 6)]
>>> 
```

This also works for tuples as input

```python
>>> a = ("Alfa","Bravo","Charlie")
>>> b = ("Delta","Echo","Foxtrot")
>>> result = zip(a,b)
>>> print(list(result))
[('Alfa', 'Delta'), ('Bravo', 'Echo'), ('Charlie', 'Foxtrot')]
>>> 
```

You can imagine you can do this for coordinates:

```python
>>> x = [1,2,3,4,5]
>>> y=  [10,20,30,40,50]
>>> coordinates = zip(x,y)
>>> print(list(coordinates))
[(1, 10), (2, 20), (3, 30), (4, 40), (5, 50)]
>>> 
```

## Unzip value using zip

You can zip and unzip with the zip() function. The example below shows both zipping and unzipping.

```python
>>> a = ("Alfa","Bravo","Charlie")
>>> b = ("Delta","Echo","Foxtrot")
>>> result = list(zip(a,b))
>>> result
[('Alfa', 'Delta'), ('Bravo', 'Echo'), ('Charlie', 'Foxtrot')]
```

Now unzip:

```python
>>> x,y = zip(*result)
>>> x
('Alfa', 'Bravo', 'Charlie')
>>> y
('Delta', 'Echo', 'Foxtrot')
>>> 
```

## Zip on other types

You can zip a <a href="https://pythonspot.com/python-strings/">string</a> and a list:

```python
>>> x = [1,2,3,4]
>>> y = "ABCD"
>>> result = list(zip(x,y))
>>> print(result)
[(1, 'A'), (2, 'B'), (3, 'C'), (4, 'D')]
```

You can zip two strings, which combines the letters as pairs:

```python
>>> x = "hello"
>>> y = "world"
>>> result = list(zip(x,y))
>>> print(result)
[('h', 'w'), ('e', 'o'), ('l', 'r'), ('l', 'l'), ('o', 'd')]
>>> 
```

Quickly generating test data?

```python
>>> x = range(10)
>>> y = range(2,20,2)
>>> print(list(zip(x,y)))
[(0, 2), (1, 4), (2, 6), (3, 8), (4, 10), (5, 12), (6, 14), (7, 16), (8, 18)]
>>> 
```

**Related links:**
* <a href="https://docs.python.org/2/library/functions.html#zip">Zip in Python docs</a>
* <a href="https://pythonbasics.org">Learn Python</a>
