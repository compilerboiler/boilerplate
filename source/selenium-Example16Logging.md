---
title: selenium Example16Logging (snippet)
date: 2020-02-13
tags: ["python"]
---
Python web automation, selenium example 'Example16Logging'


Modules used in program: 
* `import logging`
* `import time`
* `import unittest`

## Example16Logging

Python selenium example: Example16Logging

```python
from selenium import webdriver
import unittest
import time
import logging

class Example(unittest.TestCase):

    def setUp(self):
        self.driver = webdriver.Chrome("C:\\Users\\benpe\\DevMountain\\testing-resources\\chromedriver.exe")
        self.driver.implicitly_wait(20)
        self.driver.set_page_load_timeout(20)
        self.driver.maximize_window()

    def tearDown(self):
        self.driver.close()

    def test_example(self):
        #self.driver.get("")
        self.driver.implicitly_wait(10)

        #it logs it into a file
        logging.basicConfig(filename="C://Users/benpe/PycharmProjects/firstExample/test.log",
                            format='%(asctime)s: %(levelname)s: %(message)s',
                            datefmt='%m/%d/%Y %I:%M:%S %P', level=logging.DEBUG
                            )

        logging.debug("This is debug message")
        logging.info("This is info message")
        logging.warning("This is warning message")
        logging.error("This is error message")
        logging.critical("This is critical message")

        time.sleep(3)

if __name__ == '__main__':
    unittest.main()


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
