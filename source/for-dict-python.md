---
date: 2020-02-16
title: for dict python
---
In <a href="https://python.org">Python</a>, a dictionary is a key-value mapping. Every value is mapped to one key. A dictionary can have zero or more elements.

The dictionary below has 3 pairs, each pair has one value. 'a' is mapped to 1, 'b' is mapped to 2, 'c' is mapped to 3.

```python
d = {'a': 1, 'b': 2, 'c': 3}
```

You can loop over a <a href="https://pythonspot.com/python-dictionaries/">dictionary</a> using a <a href="https://pythonbasics.org/for-loops/">for loop</a>.


This works differently in Python 3 and Python 2. If you are still using Python 2, I recommend switching over to Python 3.

For Python 3.x:
```python
    for key, value in d.items():
```

For Python 2.x:
```python
    for key, value in d.iteritems():
```

## For dict example

This Python 3 example loops over the dictionary d and outputs the key value pairs from beginning to last. Keep in mind that a dictionary is not required to keep its order.

```python
d = {'a': 1, 'b': 2, 'c': 3}
for key, value in d.items():
    print(key)
    print(value)
```

If you only want the keys, you can use this code:

```python
for key in d:
    print(key)
```

To use the value without the key, just ignore the key value in:

```python
d = {'a': 1, 'b': 2, 'c': 3}
for key, value in d.items():
```

**Related links:**
* <a href="https://docs.python.org/2/tutorial/datastructures.html#dictionaries">Dictionary in Python docs</a>
* <a href="https://pythonspot.com/">Learn Python</a>

