---
tags: ["python"]
date: 2020-02-14
title: python inline if
---
In coding, you often use branching. A branch in code is executed conditionally. Without branching, you only have a list of instructions and it would always do the same, no matter what happens. 

Many programming languages support branching. <a href="https://python.org">Python</a> also supports branching. Developers speak of <a href="https://pythonbasics.org/if-statements/">if-statements</a> instead of branching. 

## Branching in Python

Python does not have a trailing if statement.
In Python there these two kinds of ifs:

* if <a href="https://pythonbasics.org/if-statements/">statements</a>

```python
if condition: statement
if condition:
    code_block
```

* if **expression** (python > 2.5)

```python
expression_if_true if condition else expression_if_false
```

You can check your Python version with 

```python
python --version
```

## If-expression

So you can do the following if expression:

```python
a = False
print("hello" if a else "world")
```

You can change the variable a to see the difference. It will return "hello" or "world" depending on the value of a.

An if-expression must always be an if-else expression, the following will throw an error because else is missing:

```python
a = False

print("hello" if a)
```

Returns if you run it:

```python
python example.py
  File "example.py", line 4
    print("hello" if a)
                      ^
SyntaxError: invalid syntax
```

So the else for the if-expression in mandatory.

**Related links:**
* <a href="https://docs.python.org/2.5/whatsnew/pep-308.html">If expressions</a>
* <a href="https://pythonbasics.org/">Learn Python</a>

