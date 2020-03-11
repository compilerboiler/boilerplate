---
title: selenium SendRequest Test (snippet)
date: 2020-02-13
tags: ["python"]
---
Python web automation, selenium example 'SendRequest Test'


Modules used in program: 
* `import unittest`

## SendRequest Test

Python selenium example: SendRequest Test

```python
from TravelingTony.Constants            import TT_Constants
from TravelingTony.pages.ContactPage    import ContactPage
from TravelingTony.BaseTestCase         import BaseTestCase
import unittest
from nose.plugins.attrib import attr

class SendRequestTest(BaseTestCase, unittest.TestCase):

    def setUp(self):
        super(SendRequestTest, self).setUp()
        self.navigate_to_page(TT_Constants['Base_URL'] + "contact")
     
    @attr(priority="high")  
    def test_SendRequestTest(self):
        contact_page_obj = ContactPage(self.driver)
        contact_page_obj.submit_request()

    @attr(priority="high") 
    def test_Validation(self):
        contact_page_obj = ContactPage(self.driver)
        contact_page_obj.validation_check()

    def tearDown(self):
        super(SendRequestTest, self).tearDown()
        

if __name__ == "__main__":
   nose.main()





```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
