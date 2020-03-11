---
title: simple Example21AssertIsNone (snippet)
date: 2020-02-12
tags: ["python"]
---
Python web automation, selenium example 'Example21AssertIsNone'


Modules used in program: 
* `import unittest`

## Example21AssertIsNone

Python selenium example: Example21AssertIsNone

```python
import unittest
from selenium import webdriver


class Test(unittest.TestCase):
    def testName(self):
        self.driver = webdriver.Chrome("C:\\Users\\benpe\\DevMountain\\testing-resources\\chromedriver.exe")
        self.assertIsNotNone(self.driver)

        self.driver = None
        self.assertIsNone(self.driver)


if __name__ == "__main__":
    unittest.main()


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
