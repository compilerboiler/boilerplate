---
date: 2020-02-16
title: unit testing python
---
---
tags: ["python"]
date: 2020-02-16
title: unit testing python
---
---
tags: ["python"]
date: 2020-02-14
title: unit testing python
---
Unit testing is a software testing method to test functions in source code. Python has a module for unit testing, <a href="https://docs.python.org/3/library/unittest.html#module-unittest">unittest</a>. 

This is different from <a href="https://pythonspot.com/python-debugging/">debugging</a>, where you already know the program is not doing what you want. 

By testing the function (unit testing) you can prevent the program from doing unexpected things. The idea is that you test both good and bad input.

The unittest module uses the idea of <a href="https://pythonbasics.org/class/">classes and objects</a>.

## Example

The program below tests the function .upper(). It compares the output to the expected output 

```python
self.assertEqual('foo.upper()', 'FOO')
```

In code that looks like this:

```python
import unittest

class TestStringMethods(unittest.TestCase):
    def test_upper(self):
        self.assertEqual('foo'.upper(), 'FOO')

if __name__ == '__main__':
    unittest.main()
```

If you run the program, it executed the test automatically:

```python
.
----------------------------------------------------------------------
Ran 1 test in 0.000s

OK
```

You can test your own functions using the unittest module.

```python
import unittest

class TestStringMethods(unittest.TestCase):

    def hello(self):
        return "hello"

    def test_upper(self):
        self.assertEqual('foo'.upper(), 'FOO')

    def test_hello(self):
        self.assertEqual(self.hello(), "hello")

if __name__ == '__main__':
    unittest.main()

```

This outputs:

```python
..
----------------------------------------------------------------------
Ran 2 tests in 0.000s

OK
```

And so the tests in are all run automatically. This means that while you code, you can run the unit tests and verify that your code still works.

**Related links:**
* <a href="https://docs.python.org/3.8/library/unittest.html">Unit test module</a>
* <a href="https://pythonbasics.org/">Learn Python</a>
