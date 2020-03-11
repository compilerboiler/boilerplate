---
title: simple Example18SkipTest (snippet)
date: 2020-02-12
tags: ["python"]
---
Python web automation, selenium example 'Example18SkipTest'


Modules used in program: 
* `import unittest`

## Example18SkipTest

Python selenium example: Example18SkipTest

```python
import unittest

class AppTesting(unittest.TestCase):

    #this will skip/ignor this test
    @unittest.SkipTest #these are called decorator
    def test_search(self):
        print("This is search test")

    #this will skip test, but print(a message)
    @unittest.skip("I am skipping this test method because it is not yet ready")
    def test_advancedSearch(self):
        print("this is advanced search method")

    #will skip on "if" condition
    @unittest.skipIf(1==1, "skip test if one is equal to one")
    def test_prepaidRecharge(self):
        print("this is prepaid recharge")

    def test_postpaidRecharge(self):
        print("this is postpaid recharge")

    def test_loginByGmail(self):
        print("this is login by eamil test")

    def test_loginByTwitter(self):
        print("this is login by twitter")


if __name__ == '__main__':
    unittest


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
