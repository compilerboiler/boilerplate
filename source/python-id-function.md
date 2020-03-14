---
tags: ["python"]
date: 2020-02-16
title: python id function
---
---
tags: ["python"]
date: 2020-02-14
title: python id function
---
[Python](https://python.org) stores all of its data in the computers memory. The memory is a block that is divided into sub blocks, where each block has an address.

![memory address](https://dev-to-uploads.s3.amazonaws.com/i/ndbhc7hlqprrter6ulz3.png)

In Python, the id() function is used to obtain the memory address of the object. 

Because Python is a high-level programming language, you usually don't need memory addresses. The value can be any [variable](https://pythonbasics.org/variables/), including a [string](https://pythonbasics.org/strings/).

The syntax of the id() function is:

```python
    id([object])
```
The parameter it takes is the object. It returns the memory address of the object. Conceptually it's the same as a memory address in C, but depending on the implementation of Python it may not be.

### Examples

The following examples show id to use:

```python
>>> x = "python"
>>> id(x)
139738512291632
>>> y = "programming"
>>> id(y)
139738511022192
>>> 
```

Python is quite smart with memory. If the value is the same, it will use the same memory address

```python
>>> x = 10
>>> y = 10
>>> z = 10
>>> id(x)
9302464
>>> id(y)
9302464
>>> id(z)
9302464
>>> 
```
These all point to the same location in memory, which is why their values are the same.

If the values are unique, the memory addresses will be different, because they point to different locations in memory:

```python
>>> x = 10
>>> y = 11
>>> z = 12
>>> id(x)
9302464
>>> id(y)
9302496
>>> id(z)
9302528
>>> 
```

**Related links:**
* [id function in docs](https://docs.python.org/3.5/library/functions.html#id)
* [Learn Python](https://gumroad.com/l/dcsp)

