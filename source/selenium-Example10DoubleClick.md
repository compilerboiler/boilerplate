---
title: simple Example10DoubleClick (snippet)
date: 2020-02-12
tags: ["python"]
---
Python web automation, selenium example 'Example10DoubleClick'


Modules used in program: 
* `import time`
* `import unittest`

## Example10DoubleClick

Python selenium example: Example10DoubleClick

```python
from selenium import webdriver
import unittest
import time
from selenium.webdriver import ActionChains


class Example(unittest.TestCase):

    def setUp(self):
        self.driver = webdriver.Chrome("C:\\Users\\benpe\\DevMountain\\testing-resources\\chromedriver.exe")
        self.driver.implicitly_wait(20)
        self.driver.set_page_load_timeout(20)
        self.driver.maximize_window()

    def tearDown(self):
        self.driver.close()

    def test_challenge(self):
        self.driver.get("https://testautomationpractice.blogspot.com")
        self.driver.implicitly_wait(10)

        element = self.driver.find_element_by_xpath('//button[@ondblclick="myFunction1()"]')

        # perform a double click on button/element
        actions = ActionChains(self.driver)
        actions.double_click(element).perform()

        time.sleep(3)

if __name__ == '__main__':
    unittest.main()


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
