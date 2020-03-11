---
title: simple assertTitle (snippet)
date: 2020-02-12
tags: ["python"]
---
Python web automation, selenium example 'assertTitle'


Modules used in program: 
* `import unittest`

## assertTitle

Python selenium example: assertTitle

```python
from selenium import webdriver

from selenium.webdriver.support.ui import WebDriverWait

from selenium.webdriver.support import expected_conditions as EC

from selenium.webdriver.common.by  import By

import unittest


class AssertTitle(unittest.TestCase):

    def setUp(self):
        global driver
        driver = webdriver.Firefox()
        driver.implicitly_wait(10)
        driver.get("http://travelingtony.weebly.com")
    
    
    def test_AssertTitle(self):
        self.assertEqual(driver.title, "Traveling Tony's Photography - Welcome")   #Should pass
        #self.assertEqual(driver.title, "Traveling John's Photography - Welcome")    #Should fail and display assertionError

    def tearDown(self):
        driver.quit()

if __name__ == "__main__":
   unittest.main()





```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
