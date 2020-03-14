---
tags: ["python"]
date: 2020-02-14
title: python try catch
---
Errors can happen if a <a href="https://python.org">Python</a> program is running. There are many types of errors, like a "couldn't open file error" or "zero division error".

If an error pops up, that doesn't mean your program should crash. 

So how do you stop it from crashing?

You can use the <a href="https://pythonbasics.org/try-except/">try-except</a> code. Other programming languages like C# or Java call this the try-catch block.

You can use this to *catch* errors (sounds better than *to except*). Some code examples listed below:

```python
try:
    for i in range(5):
        print(5/i)
except:
    print("Zero division")

print("End program")
```

For opening a file, where the filename is given as user input:

```python
>>> filename = input("Enter file:")
Enter file:test.txt
>>> try:
...     with open(filename) as f:
...         lines = f.read()
... except:
...     print("Couldn't open file")
... 
Couldn't open file
>>> 
```

Doing some maths, catch different types of exceptions:

```python
a,b=1,0
try:
    print(a/b)
    print('10'+10)
except TypeError:
    print("Cannot add, values are incompatible data types")
except ZeroDivisionError:
    print("Divided by zero")
```

You can apply this for function calls too, or inside functions.

```python
try:
    start()
    accel()
    turn()
except:
    print("Car error")
```

