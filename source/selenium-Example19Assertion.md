---
title: simple Example19Assertion (snippet)
date: 2020-02-12
tags: ["python"]
---
Python web automation, selenium example 'Example19Assertion'


Modules used in program: 
* `import unittest`

## Example19Assertion

Python selenium example: Example19Assertion

```python
import unittest
from selenium import webdriver

class Test(unittest.TestCase):
    def testName(self):
        self.driver = webdriver.Chrome("C:\\Users\\benpe\\DevMountain\\testing-resources\\chromedriver.exe")
        self.driver.get("https://www.google.com/")
        title = self.driver.title

        #assertEqual
        self.assertEqual("Google", title, "Web page title is not same")

        #this will give you an error
        #self.assertEqual("notGoogle", title, "Web page title is not the same")

        #assertNotEqual
        self.assertNotEqual("notGoogle", title, "Web page title is not the same")

if __name__ == "__main__":
    unittest.main

```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
