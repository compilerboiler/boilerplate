---
title: selenium exercise2 (snippet)
date: 2020-02-13
tags: ["python"]
---
Python web automation, selenium example 'exercise2'


Modules used in program: 
* `import test`
* `import unittest`

## exercise2

Python selenium example: exercise2

```python
from selenium import webdriver

from selenium.webdriver.support.ui import WebDriverWait

from selenium.webdriver.common.by import By 

from selenium.webdriver.support.select import Select 

import unittest

import test

class Exercise2(unittest.TestCase):

	def setUp(self):
		global driver
		driver = webdriver.Firefox()
		driver.get("http://travelingtony.weebly.com/")
		driver.maximize_window()

	#Perform search
	def test_SelectingProduct(self):
		#Locators
		searchFieldLocator = "q"
        searchButtonLocator = "span.wsite-search-button"
        turtlePictureLocator = "//div[@title='Leatherback Turtle Picture']"
        quantityDropDownLocator = "wsite-com-product-option-Quantity"

        #Finding the search field by name
        searchFieldElement = WebDriverWait(driver, 10).\
                           until(lambda driver: driver.find_element_by_name(searchFieldLocator))

        #Entering the word "leatherback" into the search field and clicking the search button
        searchFieldElement.send_keys("leatherback")
        searchButtonElement = WebDriverWait(driver, 10).until(lambda driver: driver.find_element_by_css_selector(searchButtonLocator))
        searchButtonElement.click()

        #Finding the "Leatherback Turtle Picture" product by title using Xpath
        pictureProductElement = WebDriverWait(driver, 10).until(lambda driver: driver.find_element_by_xpath(turtlePictureLocator))

        #Clicking the "Leatherback Turtle Picture" product
        pictureProductElement.click()

        #Finding the "Quantity" drop-down by id and selecting option
        quantityDropDownElement = WebDriverWait(driver, 10).until(lambda driver: driver.find_element_by_id(quantityDropDownLocator))

        Select(quantityDropDownElement).select_by_visible_text("3")

	def tearDown(self):
		driver.quit()

if __name__ == "__main__":
	unittest.main()

```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
