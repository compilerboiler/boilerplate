---
title: simple Example20AssertTrueFalse (snippet)
date: 2020-02-12
tags: ["python"]
---
Python web automation, selenium example 'Example20AssertTrueFalse'


Modules used in program: 
* `import unittest`

## Example20AssertTrueFalse

Python selenium example: Example20AssertTrueFalse

```python
import unittest
from selenium import webdriver

class Test(unittest.TestCase):
    def testName(self):
        self.driver = webdriver.Chrome("C:\\Users\\benpe\\DevMountain\\testing-resources\\chromedriver.exe")
        self.driver.get("https://google.com")

        title = self.driver.title

        self.assertTrue(title == "Google")

        self.assertFalse(title == "Not Google")

if __name__ == "__main__":
    unittest.main()

```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
