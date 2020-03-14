---
date: 2020-02-16
title: custom exception in python
---
<a href="https://python.org">Python</a> Applications may call custom exceptions by creating a brand new exception class. Custom Exceptions need to be derived from the `Exception` class.

## What is an Exception?

An exception can be thrown with the `raise` keyword. They can be handled with the <a href="https://pythonprogramminglanguage.com/try-except/">try-catch</a> block.

You can try this in the Python shell, by typing `raise Exception("your message")`.

    ➜  ~ python3
    Python 3.7.5 (default, Nov 20 2019, 09:21:52) 
    [GCC 9.2.1 20191008] on linux
    Type "help", "copyright", "credits" or "license" for more information.
    >>> raise Exception("No can do")
    Traceback (most recent call last):
      File "<stdin>", line 1, in <module>
    Exception: No can do
    >>> 

All built-in exceptions use the `Exception` class. User-defined exceptions should be derived from this class (<a href="https://pythonbasics.org/inheritance/">inherited</a>).

## Custom Exception

The program shown below creates a custom exception `HappyError` that inherits from the `Exception` class.

```python
class HappyError(Exception):
    pass

raise HappyError("To happy to run")
```

The above program then raises the `HappyError` exception:

    ➜  ~ python3 program.py
    Traceback (most recent call last):
      File "t.py", line 5, in <module>
        raise HappyError("To happy to run")
    __main__.HappyError: To happy to run

Many modules define their own exceptions.

Optionally you can override the <a href="https://pythonbasics.org/constructor/">constructor</a> like this:

```python
class ValidationError(Exception):
    def __init__(self, message, errors):

        # Call the base class constructor with the parameters it needs
        super().__init__(message)

        # Now for your custom code...
        self.errors = errors
```

But with Python 3 Exceptions, you don't need to do override anything. If all you want is an informative message for your exception, do this:

```python
class MyException(Exception):
    pass

raise MyException("My car is swimming")
```
