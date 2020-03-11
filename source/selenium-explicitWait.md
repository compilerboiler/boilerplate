---
title: selenium explicitWait (snippet)
date: 2020-02-13
tags: ["python"]
---
Python web automation, selenium example 'explicitWait'


## explicitWait

Python selenium example: explicitWait

```python
from selenium import webdriver
from selenium.webdriver.support.ui import WebDriverWait
from selenium.webdriver.support import expected_conditions as EC 
from selenium.webdriver.common.by import By 

driver = webdriver.Firefox()

driver.get("http://google.com")

fLocator = "input[name=q]"

try:
	searchField = WebDriverWait(driver, 10).until(EC.presence_of_element_located((By.CSS_SELECTOR, fLocator)))

	#Why doesn't this work? It says "TypeError: __init__() takes exactly 2 arguments (3 given)"
#	searchField = WebDriverWait(driver, 10).until(EC.presence_of_element_located(By.CSS_SELECTOR, fLocator))
finally:
	driver.quit()

```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
