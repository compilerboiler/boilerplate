---
title: simple Example2RadioButtonAndCheckBoxes (snippet)
date: 2020-02-12
tags: ["python"]
---
Python web automation, selenium example 'Example2RadioButtonAndCheckBoxes'


Modules used in program: 
* `import time`
* `import unittest`

## Example2RadioButtonAndCheckBoxes

Python selenium example: Example2RadioButtonAndCheckBoxes

```python
from selenium import webdriver
import unittest
import time


class Example(unittest.TestCase):

    def setUp(self):
        self.driver = webdriver.Chrome("C:\\Users\\benpe\\DevMountain\\testing-resources\\chromedriver.exe")
        self.driver.implicitly_wait(20)
        self.driver.set_page_load_timeout(20)
        self.driver.maximize_window()

    def tearDown(self):
        self.driver.close()

    def test_challenge(self):
        self.driver.get("https://fs2.formsite.com/meherpavan/form2/index.html?1537702596407")
        self.driver.implicitly_wait(10)

        #the status of the button
        status = self.driver.find_element_by_xpath('(//label[@for="RESULT_RadioButton-7_0"])').is_selected()
        print("Selected: ", status)
        time.sleep(2)

        #clicking on the button
        self.driver.find_element_by_xpath('(//label[@for="RESULT_RadioButton-7_0"])').click()
        time.sleep(2)

        #the status of the button after you click on it
        status2 = self.driver.find_element_by_xpath('(//label[@for="RESULT_RadioButton-7_0"])').is_enabled()
        print("Selected: ", status2)

        #clicking on the check boxes
        self.driver.find_element_by_xpath('(//label[@for="RESULT_CheckBox-8_0"])').click()
        self.driver.find_element_by_xpath('(//label[@for="RESULT_CheckBox-8_6"])').click()

        time.sleep(3)


if __name__ == '__main__':
    unittest.main()


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
