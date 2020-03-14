---
tags: ["python"]
date: 2020-02-16
title: python dictionary examples
---
---
tags: ["python"]
date: 2020-02-14
title: python dictionary examples
---
The [Python](https://python.org) language supports many types of variables. One of those types is a dictionary, this is similar to a [hash map](https://en.wikipedia.org/wiki/Hash_table) in computer science.

So another variable is the [dictionary](https://pythonprogramminglanguage.com/dictionary/): a container model, it can store any type of object.

Each dictionary key maps a value (`key => value`) to (`:`) divided by a colon, comma between each pair (**, **), in the entire dictionary is between curly braces (`{` `}`) 

This lets you quickly retrieve a value, given a key. There are many scenarios in which that is useful. Like a map of phone numbers, internet addresses or to keep track of word frequency.

![hashmap](https://dev-to-uploads.s3.amazonaws.com/i/e39a80s35e1qptvxxo01.jpeg)

If new to Python, you may like this [Python course](https://gumroad.com/l/dcsp)

## Dictionary example

The following format:

```python
    d = {key1: value1, key2: value2}
```

Key must be unique, but the value is not necessarily unique.

A value may take any data type, but the key must be immutable, such as [strings](https://pythonbasics.org/strings/), [numbers](https://docs.python.org/2.4/lib/typesnumeric.html), or [tuples](https://pythonprogramminglanguage.com/tuples/).

A simple example dictionary:

```python
    dict = { 'Alice': '2341', 'Beth': '9102', 'Cecil': '3258'}
```
So also create a dictionary:
```python
    dict1 = { 'abc': 456};
    dict2 = { 'abc': 123, 98.6: 37};
```

## to access the dictionary values

Use the appropriate key in the familiar square brackets, as shown in the following examples:

```python
dict = { 'Name': 'Zara', 'Age': 7, 'Class': 'First'}
 
print("dict ['Name']:", dict['Name'])
print("dict ['Age']:", dict['Age'])
```

Examples of the above output:
```python
dict ['Name']: Zara
dict ['Age']: 7
```

If there are no keys to access the data dictionary, it will output the following error:
```python
dict = { 'Name': 'Zara', 'Age': 7, 'Class': 'First'}
print("dict [ 'Alice']:", dict [ 'Alice'])
```
Examples of the above output:
```python
    dict [ 'Zara']:
    Traceback (most recent call last):
      File "test.py", line 4, in <module>
        print "dict ['Alice']:", dict ['Alice'];
    KeyError: 'Alice'
```
## Modifying a dictionary

A way to add new content to the dictionary is to add new key / value pairs, modify, or delete existing key / value pairs like in the following examples:
```python
mydict = { 'Name': 'Zara', 'Age': 7, 'Class': 'First'};

mydict['Age'] = 8; # update existing entry                                                            
mydict['School'] = "ABC School"; # Add new entry                                                      

print("dict['Age']:", mydict['Age'])
print("dict['School']:", mydict['School'])
```

Examples of the above output:

```python
dict['Age']: 8
dict['School']: ABC School
```

## Delete dictionary elements

You can delete a single element with just one statement. Delete a dictionary with the del command, as in the following examples:

```python
mydict = { 'Name': 'Zara', 'Age': 7, 'Class': 'First'};

del mydict [ 'Name']; # delete key is 'Name' entry                                                    
mydict.clear (); # Clear all dictionary entries                                                       
del mydict; # delete dictionary                                                                       

print("dict [ 'Age']:", mydict['Age'])
print("dict [ 'School']:", mydict['School'])
```

But this raises an exception, because there is no longer a dictionary (deleted the whole dictionary with the `del` statement):

```python
Traceback (most recent call last):
  File "tmp.py", line 7, in <module>
    print("dict [ 'Age']:", mydict['Age'])
NameError: name 'mydict' is not defined
```

**key characteristics of the dictionary**

Dictionary may take any [python object](https://pythonbasics.org/class/), or may be user-defined, but not the key.

Two important points to remember:

1) Python does not allow the same key appears twice. When you create the same key twice, the last value will be remembered, like the following examples thas the key Name twice:

```python
mydict = { 'Name': 'Zara', 'Age': 7, 'Name': 'Manni'}
print("dict['Name']:", mydict['Name'])
```

Examples of the above output:

```python
    dict['Name']: Manni
```

2) key must not be changed, it is possible to use a number, string, or act as a tuple, but it will not work with the list, examples:

```python
mydict = {['Name']: 'Zara', 'Age': 7}
print("dict['Name']:", mydict ['Name'])
```

Examples of the above output:

```python
Traceback (most recent call last):
  File "tmp.py", line 2, in <module>
    mydict = {['Name']: 'Zara', 'Age': 7}
TypeError: unhashable type: 'list'
```

## dictionaries built-in functions & methods

Python dictionary contains the following built-in functions:

No. | function and description
--- | ---
1 | `cmp(dict1, dict2)` Comparison of two dictionary elements.
2 | `len(dict)` Counting the number of dictionary elements, i.e., the total number of keys.
3 | `str(dict)` String dictionary printable output representation.
4 | `type(variable)` The return type of a variable input, if the variable is a dictionary returns a dictionary.

Python dictionary contains the following built-in functions:

No. | function and description
--- | ---
1 | `.clear()` Delete all the elements in the dictionary
2 | `.copy()` Returns a shallow copy of the dictionary
3 | `.fromkeys()` Create a new dictionary, a sequence of elements do seq dictionary key, val is a dictionary of all the key corresponding to the initial value
4 | `.get(key, default = None)` Returns the value of the specified key, if the value is not in the dictionary to return default values
5 | `.has_key(key)` If the key is in the dictionary dict returns true, otherwise returns false
6 | `.items ()` In return may traverse the list (key, value) tuples array
7 | `.keys()` To return a list of all the keys dictionary
8 | `.setdefault(key, default = None)` And get () is similar, but if the key does not already exist in the dictionary, it will add key and value to default
9 | `.update(dict2)` Dict2 the dictionary of key / value pairs in the update to the dict
10 | `.values​()` To return a list of all the values ​​in the dictionary


