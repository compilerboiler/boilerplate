---
title: simple Example23AssertGreaterAndAssertLess (snippet)
date: 2020-02-12
tags: ["python"]
---
Python web automation, selenium example 'Example23AssertGreaterAndAssertLess'


Modules used in program: 
* `import unittest`

## Example23AssertGreaterAndAssertLess

Python selenium example: Example23AssertGreaterAndAssertLess

```python
import unittest


class Test(unittest.TestCase):
    def testName(self):
        self.assertGreater(100, 10) #is the first value greater than the second value?
        self.assertLess(10, 100) #is the first value less than the second value?
        self.assertGreaterEqual(100, 100) #is the first value greater or euqal than the second value?
        self.assertLessEqual(10, 10)    #is the first value less or equal than the second value?


if __name__ == "__main__":
    unittest.main()


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
