---
title: python-code-clone-list (snippet)
date: 2020-02-15
tags: ["python"]
---
Python example 'python-code-clone-list'


Modules used in program: 
* `import copy`

## python-code-clone-list

Python code example: python-code-clone-list

```python
my_list = [27, 13, -11, 60, 39, 15]

# Clone a list by brute force
my_duplicate_list = [item for item in my_list]

# Clone a list with a slice
my_duplicate_list = my_list[:]

# Clone a list with the list constructor
my_duplicate_list = list(my_list) 

# Clone a list with the copy function (Python 3.3+)
my_duplicate_list = my_list.copy() # preferred method

# Clone a list with the copy package
import copy
my_duplicate_list = copy.copy(my_list)
my_deep_duplicate_list = copy.deepcopy(my_list)

# Clone a list with multiplication?
my_duplicate_list = my_list * 1 # do not do this


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org

More Python: https://pythonprogramminglanguage.com
