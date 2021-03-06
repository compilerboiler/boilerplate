---
title: selenium SendRequestTest (snippet)
date: 2020-02-13
tags: ["python"]
---
Python web automation, selenium example 'SendRequestTest'


Modules used in program: 
* `import time`
* `import unittest`

## SendRequestTest

Python selenium example: SendRequestTest

```python
from TravelingTony.Constants            import TT_Constants
from TravelingTony.BaseTestCase         import BaseTestCase
#from TravelingTony.Common               import Common
from TravelingTony.pages.ContactPage    import ContactPage
import unittest
import time


class SendRequestTest(BaseTestCase, unittest.TestCase):

    def setUp(self):
        super(SendRequestTest, self).setUp()
        self.navigate_to_page(TT_Constants['Base_URL'] + "contact")
        

    def test_SendRequestTest(self):
        contact_page_obj = ContactPage(self.driver)
        contact_page_obj.submit_request()
        # common_obj = Common(self.driver)
        # common_obj.wait_for_element_visibility(10, 
        #                                        "xpath", 
        #                                        "//input[contains(@name, 'first')]"
        # )
        # common_obj.fill_out_field("xpath", 
        #                           "//input[contains(@name, 'first')]", 
        #                           "Paul"
        # )
        # common_obj.fill_out_field("xpath", 
        #                           "//input[contains(@name, 'last')]", 
        #                           "Pierce"
        # )
        # common_obj.fill_out_field("xpath", 
        #                           "(//input[contains(@id, 'input')])[3]", 
        #                           "contactemail@test.com"
        # )
        # common_obj.fill_out_field("xpath", "//textarea", "My comment")
        # common_obj.click(10, "xpath", "//span[.='Submit']")
        # common_obj.wait_for_element_visibility(10, 
        #                                        "xpath", 
        #                                        "//div[contains(text(), 'Thank you')]"
        # )

        """
        Just using time.sleep() so that you see the last webdriver action.
        I do not recommend using this in your tests.
        """
        time.sleep(5)

    def test_Validation(self):
        contact_page_obj = ContactPage(self.driver)
        contact_page_obj.validation_check()
        """
        Just using time.sleep() so that you see the last webdriver action.
        I do not recommend using this in your tests.
        """
        time.sleep(5)
    
    def tearDown(self):
        super(SendRequestTest, self).tearDown()
        

if __name__ == "__main__":
   unittest.main()





```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
