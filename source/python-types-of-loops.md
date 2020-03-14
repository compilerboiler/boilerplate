---
date: 2020-02-16
title: python types of loops
---
---
tags: ["python"]
date: 2020-02-16
title: python types of loops
---
---
tags: ["python"]
date: 2020-02-14
title: python types of loops
---
In this article we introduce Python's loop, the program in general are executed sequentially. Sequentially means in sequential order (top down):

```
do A
do B
do C
```

In a variety of programming languages, control structures allows for more complex execution paths.

Loop allows us to perform a statement or group of statements *repeatedly*, the following is the general form in most programming languages ​​loop statement:

![python loop](https://dev-to-uploads.s3.amazonaws.com/i/urxflqstc9x0qipigomi.jpg)

Python is provided for and while loops (not do..while loop in Python):

Circulation type | Description
--- | ---
[The while loop](https://pythonprogramminglanguage.com/while-loop/) | determines the given condition is true. When the execution loop, or exit the loop.
[For loop](https://pythonbasics.org/for-loops/) | Repeat statement
[Nested loop] | You can be nested for loop while loop body

The while loop in code:

```python
>>> index = 0
>>> n = 10
>>> while index < n:
...     print(index)
...     index = index + 1
... 
0
1
2
3
4
5
6
7
8
9
```

The for loop:

```python
>>> for i in range(1,3):
...     print(i)
... 
1
2
```

The nested for loop:

```python
>>> 
>>> for x in range(1,10):
...     for y in range(1,10):
...         print(f"({x},{y})")
```

## loop control statements

Loop control statements can change the order of statement execution. Python loop control supports the following statement:

Control statements | Description
--- | ---
[Break Statement](https://dev.to/libertycodervice/python-break-statement-4ki5) | Terminates the loop during the execution of statement block, and jump out of the entire cycle
[Continue Statement](https://dev.to/libertycodervice/python-continue-statement-dme) | Terminates the current execution loop statement block, out of the cycle, the next cycle execution.
Pass sentence | pass an empty statement, in order to maintain the integrity of the program structure.
