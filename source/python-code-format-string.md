---
title: python-code-format-string (snippet)
date: 2020-02-15
tags: ["python"]
---
Python example 'python-code-format-string'


## python-code-format-string

Python code example: python-code-format-string

```python
name = "Jeremy"
age = 25

# String formatting using concatenation
print("My name is " + name + ", and I am " + str(age) + " years old.")

# String formatting using multiple prints
print("My name is ", end="")
print(name, end="")
print(", and I am ", end="")
print(age, end="")
print(" years old.")

# String formatting using join
print(''.join(["My name is ", name, ", and I am ", str(age), " years old"]))

# String formatting using modulus operator
print("My name is %s, and I am %d years old." % (name, age))

# String formatting using format function with ordered parameters
print("My name is {}, and I am {} years old".format(name, age))

# String formatting using format function with named parameters
print("My name is {n}, and I am {a} years old".format(a=age, n=name))

# String formatting using f-Strings (Python 3.6+)
print(f"My name is {name}, and I am {age} years old")


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org

More Python: https://pythonprogramminglanguage.com
