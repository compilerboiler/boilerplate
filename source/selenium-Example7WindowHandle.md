---
title: simple Example7WindowHandle (snippet)
date: 2020-02-12
tags: ["python"]
---
Python web automation, selenium example 'Example7WindowHandle'


Modules used in program: 
* `import time`
* `import unittest`

## Example7WindowHandle

Python selenium example: Example7WindowHandle

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
        self.driver.get("http://demo.automationtesting.in/Windows.html")
        self.driver.implicitly_wait(10)

        self.driver.find_element_by_xpath('(//button[@class="btn btn-info"])[1]').click()

        print("My Current window handle: ", self.driver.current_window_handle)

        #returns all the handle values of opened browser windows
        handles = self.driver.window_handles

        for handle in handles:
            self.driver.switch_to_window(handle)
            print(self.driver.title)
            if self.driver.title == "Frames & windows":
                self.driver.close() #close only parent browser


        time.sleep(3)

if __name__ == '__main__':
    unittest.main()


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
