---
title: selenium Example14HowToDownloadFileInChrome (snippet)
date: 2020-02-13
tags: ["python"]
---
Python web automation, selenium example 'Example14HowToDownloadFileInChrome'


Modules used in program: 
* `import time`
* `import unittest`

## Example14HowToDownloadFileInChrome

Python selenium example: Example14HowToDownloadFileInChrome

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
        self.driver.get("http://demo.automationtesting.in/FileDownload.html")
        self.driver.implicitly_wait(10)

        #download text file
        self.driver.find_element_by_xpath('//textarea[@id="textbox"]').send_keys("Testing")
        self.driver.find_element_by_xpath('//button[@id="createTxt"]').click() #generate file button
        self.driver.find_element_by_xpath('//a[@download="info.txt"]').click() #download link

        time.sleep(3)

if __name__ == '__main__':
    unittest.main()


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
