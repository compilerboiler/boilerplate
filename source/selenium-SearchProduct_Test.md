---
title: selenium SearchProduct Test (snippet)
date: 2020-02-13
tags: ["python"]
---
Python web automation, selenium example 'SearchProduct Test'


Modules used in program: 
* `import nose`
* `import unittest`

## SearchProduct Test

Python selenium example: SearchProduct Test

```python
from TravelingTony.Constants               import TT_Constants
from TravelingTony.pages.WelcomePage       import WelcomePage
from TravelingTony.BaseTestCase            import BaseTestCase
import unittest
import nose
from nose.plugins.attrib import attr

class SearchProductTest(BaseTestCase, unittest.TestCase):

    def setUp(self):
        super(SearchProductTest, self).setUp()
        self.navigate_to_page(TT_Constants['Base_URL'])
        
    @attr(priority="high")
    def test_SearchProductTest(self):
        welcome_page_obj = WelcomePage(self.driver)
        welcome_page_obj.search("leatherback")
        

    def tearDown(self):
        super(SearchProductTest, self).tearDown()
        

if __name__ == "__main__":
   nose.main()





```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
