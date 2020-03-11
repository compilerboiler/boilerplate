---
title: simple Example15CaptureScreenShots (snippet)
date: 2020-02-12
tags: ["python"]
---
Python web automation, selenium example 'Example15CaptureScreenShots'


Modules used in program: 
* `import time`
* `import unittest`

## Example15CaptureScreenShots

Python selenium example: Example15CaptureScreenShots

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
        self.driver.get("http://newtours.demoaut.com/mercurywelcome.php")
        self.driver.implicitly_wait(10)

        #first way to screen shot
        self.driver.save_screenshot("C://Users/benpe/PycharmProjects/firstExample/ScreenShots/homepage.png")

        #second way to screen shot
        self.driver.get_screenshot_as_file("C://Users/benpe/PycharmProjects/firstExample/ScreenShots/homepage2.png")

        time.sleep(3)

if __name__ == '__main__':
    unittest.main()


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
