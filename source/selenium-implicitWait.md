---
title: simple implicitWait (snippet)
date: 2020-02-12
tags: ["python"]
---
Python web automation, selenium example 'implicitWait'


## implicitWait

Python selenium example: implicitWait

```python
from selenium import webdriver

#Should run to completion
# driver = webdriver.Firefox()

# driver.implicitly_wait(15)

# driver.get("http://google.com")

# searchField = driver.find_element_by_css_selector("input[name=q")

# driver.quit()

#Should timeout after ~ 15 s
driver1 = webdriver.Firefox()

driver1.implicitly_wait(15)

driver1.get("http://google.com")

#searchField = driver1.find_element_by_css_selector("input[name=d")

searchField = driver.find_element_by_css_selector("input[name=q")

driver.quit()

```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
