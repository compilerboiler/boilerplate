---
tags: ["python"]
date: 2020-02-16
title: sort python dictionary
---
---
tags: ["python"]
date: 2020-02-14
title: sort python dictionary
---
In <a href="https://python.org">Python</a> a dictionary is a <a href="https://pythonbasics.org/dictionary/">key-value mapping</a>. Its a set of key-value pairs, every key has a value.

You can use this to <a href="https://pythonspot.com/python-dictionaries/">receive values using keys</a>. Values in a dictionary can be of any data type. The data in a dictionary is not in any specific order.

This means you can define a dict with key-value pairs like this:

```python
>>> di = { 'five': 5, 'two': 2, 'one': 1 }
>>> di
{'five': 5, 'two': 2, 'one': 1}
>>> 
```

You can call the list method with the dictionary as parameter. This outputs all the keys:

```python
>>> list(di)
['five', 'two', 'one']
```

## Sort dictionary by values

Each pair in a dictionary is a key-value pair. For the dictionary above 'five','two' and 'one' are keys. The values are 1,2,5 and each are mapped. 

To sort a dictionary by values you can use:

```python
>>> sorted(di.values())
[1, 2, 5]
```

## Sort dict by keys

You can sort by keys too:

```python
>>> sorted(di)
['five', 'one', 'two']
```

This is in alphabetic order, 'f' before 'o' and 't'.

## Real world example

You can define a dictionary with months like this:

```python
>>> month = { 'January':1, 'February':2, 'March':3, 'April':4, 'May':5, 'June':6 }
```

Then you can sort by keys or values:

```python
>>> sorted(month)
['April', 'February', 'January', 'June', 'March', 'May']
>>> sorted(month.values())
[1, 2, 3, 4, 5, 6]

```

You can sort in reverse order too:

```python
>>> sorted(month, reverse=True)
['May', 'March', 'June', 'January', 'February', 'April']
```

**Related links:**
* <a href="https://pythonbasics.org/dictionary/">Python dictionary</a>
* <a href="https://wiki.python.org/moin/HowTo/Sorting">More on sorting in Python</a>
* <a href="https://pythonbasics.org">Learn Python</a>


