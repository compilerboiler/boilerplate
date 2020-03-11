---
title: selenium Example11RightClick (snippet)
date: 2020-02-13
tags: ["python"]
---
Python web automation, selenium example 'Example11RightClick'


Modules used in program: 
* `import time`
* `import unittest`

## Example11RightClick

Python selenium example: Example11RightClick

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
        self.driver.get("https://swisnl.github.io/jQuery-contextMenu/demo.html")
        self.driver.implicitly_wait(10)

        button = self.driver.find_element_by_xpath('//span[@class="context-menu-one btn btn-neutral"]')

        #perform right click action
        actions = ActionChains(self.driver)
        actions.context_click(button).perform()

        time.sleep(3)

if __name__ == '__main__':
    unittest.main()


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
