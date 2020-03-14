---
date: 2020-02-16
title: python lists
---
[Python](https://python.org) sequence is the most basic data structure. Each element in the sequence is assigned a number - its position, or index, the first index is 0, the second index is 1, and so on.

Python has a built-in type 6 sequences, but the most common are [lists](https://pythonbasics.org/list/) and [tuples](https://pythonprogramminglanguage.com/tuples/).

A sequence of operations can be carried out, including indexing, slicing, add, multiply, check members.

Further, Python already has built-in methods for sequence length, the maximum and minimum element. You may like [this Python course](https://gumroad.com/l/dcsp)

## List

Python list is one of the most common types of data. It appears as a comma-separated values ​​in square brackets.

Create a list, as long as the comma-separated data items using different brackets can be as follows:

```python
>>> list1 = [ 'physics', 'chemistry', 1997, 2000]
>>> list2 = [1, 2, 3, 4, 5]
>>> list3 = [ "a", "b", "c", "d"]
>>> 
```

Like string indices, list indices start at 0. The list can be intercepted, combinations and the like.

## Access list values

The index is used to access the values ​​in the list, as follows:

```python
>>> list1 = [ 'physics', 'chemistry', 1997, 2000]
>>> list2 = [1, 2, 3, 4, 5]
>>> print(list1[0])
physics
>>> print(list2[0])
1
>>> print(list1[1:3])
['chemistry', 1997]
>>> print(list2[1:3])
[2, 3]
>>> 
```

## update list

You can modify or update data items in the list, you can also add a list item using append() method, as follows:

```python
>>> list1 = [ 'physics', 'chemistry', 1997, 2000]
>>> list1[2] = 2010
>>> list1
['physics', 'chemistry', 2010, 2000]
>>> 
>>> list1.append("Tango")
```

## Delete list elements

You can use the `del` statement to delete the list of elements, the following examples:

```python
>>> list1 = [ 'physics', 'chemistry', 1997, 2000]
>>> list1
['physics', 'chemistry', 1997, 2000]
>>> del list1[1]
>>> list1
['physics', 1997, 2000]
>>> 
```

## Python script operator list

Similar lists of + and * operators string. + Number combination for the list, the list for repeatedly asterisk.

As follows:

Python expressions | result | Description
--- | --- | ---
len ([1, 2, 3]) | 3 | length
[1, 2, 3] + [4, 5, 6] | [1, 2, 3, 4, 5, 6] | composition
[ 'Hi!'] * 4 | [ 'Hi!', 'Hi!', 'Hi!', 'Hi!'] | Repeat
3 in [1, 2, 3] | True | element exists in the list
for x in [1, 2, 3]: print x, | 1 2 3 | iteration

## Python interception list

Python list operation type string taken as follows:

```python
    L = [ 'spam', 'Spam', 'SPAM!']
```

operating:

Python expressions | result | Description
--- | --- | ---
L [2] | 'SPAM!' | Third element in the list is read
L [-2] | 'Spam' | penultimate read list element
L [1:] | [ 'Spam', '! SPAM'] | taken from the second list element start

## Python list of functions & methods

Python includes the following functions:

No. | function
--- | ---
1 | cmp(list1, list2) Compare the two lists of elements
2 | len(list) The number of list elements
3 | max(list) Returns a list of elements of the maximum
4 | min(list) Returns a list of elements of the minimum
5 | list(seq) Convert a list of tuples

Python includes the following methods:

No. | Methods
--- | ---
1 | list.append(obj) Add new object at the end of the list
2 | list.count(obj) The number of times an element statistics appear in the list
3 | list.extend(seq) A plurality of values ​​in another sequence added at the end of the list of one-time (with a new list of the original extended list)
4 | list.index(obj) A value index to find the location of the first match from the list
5 | list.insert(index, obj) Inserting objects list
6 | list.pop(obj = list [-1]) Removing one element in the list (default to the last element), and returns the value of the element
7 | list.remove(obj) Remove the list a value of the first match
8 | list.reverse()  Reverse elements in the list
9 | list.sort([func]) The original list is sorted

More reading:
* [Data structures in Python](https://docs.python.org/3/tutorial/datastructures.html)
* [Python list examples](https://pythonbasics.org/list/)

