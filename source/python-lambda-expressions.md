---
date: 2020-02-16
title: python lambda expressions
---
---
tags: ["python"]
date: 2020-02-16
title: python lambda expressions
---
---
tags: ["python"]
date: 2020-02-14
title: python lambda expressions
---

You can create small anonymous functions in <a href="https://python.org">Python</a> using *the lambda keyword*. 

By anonymous I mean it doesn't need to have a name, normal <a href="https://pythonbasics.org/functions/">functions</a> start with the *def* keyword and require a name.A lambda expression is not a statement, it returns a value.

Lets say you want a function that returns the sum of its two arguments
Imagine you have a simple function like this:

```python

def sum(a,b):
    return a+b
```
That is quite a lot to write. 

## Lambda expressions

Instead you can create a lambda expression like the example below. 
A lambda function that adds two variables as an argument and prints the result:

```python
lambda a, b: a+b
```

You can then use it like this:

```python
>>> f = lambda a,b : a+b
>>> f(2,3)
5
>>> f(10,15)
25
>>> 
```

You can create all kinds of lambda expressions, this is a lot shorter to write than creating functions for tiny operations.

```python

# A lambda function that adds 10 to the argument
x = lambda a : a + 10
print(x(8))

# A lambda function that multiplies two variables
x = lambda a, b : a * b
print(x(8, 9))

# A lambda function that sums its arguments
x = lambda a, b, c : a + b + c
print(x(1, 2, 3))
```

