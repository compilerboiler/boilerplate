---
title: selenium exercise4 (snippet)
date: 2020-02-13
tags: ["python"]
---
Python web automation, selenium example 'exercise4'


Modules used in program: 
* `import time`
* `import unittest`

## exercise4

Python selenium example: exercise4

```python
from selenium                                       import webdriver

from selenium.webdriver.support.ui                  import WebDriverWait

from selenium.webdriver.common.by                   import By

from selenium.webdriver.common.action_chains        import ActionChains

from selenium.webdriver.common.keys                 import Keys

import unittest

import time


class selectOption(unittest.TestCase):

    def setUp(self):
        global driver
        driver = webdriver.Firefox()
        driver.get("http://travelingtony.weebly.com/store/p1/Leatherback_Turtle_Picture.html")
        driver.maximize_window()
    
    
    
    def test_selectOption(self):
        #Locators
        dropDownID           = "wsite-com-product-option-Quantity"
        dropDownElement      = WebDriverWait(driver, 10).\
                               until(lambda driver: driver.find_element_by_id(dropDownID))
        
        
        actions = ActionChains(driver)
        actions.send_keys_to_element(dropDownElement, Keys.ENTER)
        actions.send_keys(Keys.ARROW_DOWN)
        actions.send_keys(Keys.ARROW_DOWN)
        actions.perform()
        # Just using time.sleep() so that you can see the last webdriver action. I do not recommend using it in your tests
        time.sleep(10)


    def tearDown(self):
        driver.quit()

if __name__ == "__main__":
   unittest.main()





```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
