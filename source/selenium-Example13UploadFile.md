---
title: simple Example13UploadFile (snippet)
date: 2020-02-12
tags: ["python"]
---
Python web automation, selenium example 'Example13UploadFile'


Modules used in program: 
* `import time`
* `import unittest`

## Example13UploadFile

Python selenium example: Example13UploadFile

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

    def test_example(self):
        self.driver.get("https://testautomationpractice.blogspot.com")
        self.driver.implicitly_wait(10)

        #gotta switch to a different frame to work
        self.driver.switch_to_frame(0)

        self.driver.find_element_by_xpath('//input[@type="file"]').send_keys('C://Users/benpe/Desktop/Screenshot_1558289769.png')

        time.sleep(3)

if __name__ == '__main__':
    unittest.main()


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
