---
tags: ["python"]
date: 2020-02-16
title: exponents in python
---
---
tags: ["python"]
date: 2020-02-14
title: exponents in python
---
You can use exponents in <a href="https://python.org">Python</a>, without using any modules. Let's see an example. To raise 3 squared, would look like this:

```python
    >>> 3**2
    9
```

Easy. So when using a single * it's multiplication, when using two ** it's raised.

To get 2 to the power of 3, you would use:

```python
    >>> 2**3
    8
```

## Raise many

To get a lot of exponents, you can use it combined with a for loop:

```python
    >>> for i in range(1,10):
    ...     3**i
    ... 
    3
    9
    27
    81
    243
    729
    2187
    6561
    19683
```

In these examples I'm using the <a href="https://pythonprogramminglanguage.com/repl/">Python interpreter</a>, you can <a href="https://pythonbasics.org/execute-python-scripts/">run it in code</a> too. But then you have to print the output.

```python
    x = 2**3
    print(x)
```

## Explicit output

You can output variables together with text like this:

```python
    for i in range(0,10):
        print("Exponent, 3 to the power of",i,"=",3**i)
```

This outputs the data in more descriptive terms:

```python
Exponent, 3 to the power of 0 = 1
Exponent, 3 to the power of 1 = 3
Exponent, 3 to the power of 2 = 9
Exponent, 3 to the power of 3 = 27
Exponent, 3 to the power of 4 = 81
Exponent, 3 to the power of 5 = 243
Exponent, 3 to the power of 6 = 729
Exponent, 3 to the power of 7 = 2187
Exponent, 3 to the power of 8 = 6561
Exponent, 3 to the power of 9 = 19683
```

**Related links:**
* <a href="https://python.org">Official Python site</a>
* <a href="https://pythonbasics.org">Learn Python</a>

