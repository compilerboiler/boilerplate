---
title: selenium waitForElements (snippet)
date: 2020-02-13
tags: ["python"]
---
Python web automation, selenium example 'waitForElements'


Modules used in program: 
* `import unittest`

## waitForElements

Python selenium example: waitForElements

```python
from selenium import webdriver

from selenium.webdriver.support.ui import WebDriverWait

from selenium.webdriver.support import expected_conditions as EC

from selenium.webdriver.common.by  import By

import unittest


class WaitForElements(unittest.TestCase):

    def setUp(self):
        global driver
        driver = webdriver.Firefox()
        driver.get("http://travelingtony.weebly.com")
    
    
    def test_WaitForCheckOutPhotosButton(self):
        bLocator = "//span[.='Check out my coolest photos']"
        seebutton = WebDriverWait(driver, 10).until(EC.presence_of_element_located((By.XPATH, bLocator)))

    def test_WaitForSearchField(self):
        sLocator = "input.wsite-search-input"
        sField = WebDriverWait(driver, 10).until(EC.presence_of_element_located((By.CSS_SELECTOR, sLocator)))

    def tearDown(self):
        driver.quit()

if __name__ == "__main__":
   unittest.main()





```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
