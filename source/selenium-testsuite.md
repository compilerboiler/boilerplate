---
title: simple testsuite (snippet)
date: 2020-02-12
tags: ["python"]
---
Python web automation, selenium example 'testsuite'


Modules used in program: 
* `import unittest`

## testsuite

Python selenium example: testsuite

```python
import unittest

from testcase1 import TestCase1

from testcase2 import TestCase2

class TestSuite(unittest.TestSuite):
  
  def suite():
      suite = unittest.TestSuite()
      suite.addTest(TestCase1('test_waitForCheckoutPhotosButton'))
      suite.addTest(TestCase2('test_waitForSearchField'))
      return suite

if __name__ == "__main__":
   unittest.main()


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
