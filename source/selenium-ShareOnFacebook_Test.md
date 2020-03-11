---
title: simple ShareOnFacebook Test (snippet)
date: 2020-02-12
tags: ["python"]
---
Python web automation, selenium example 'ShareOnFacebook Test'


Modules used in program: 
* `import nose`
* `import unittest`

## ShareOnFacebook Test

Python selenium example: ShareOnFacebook Test

```python
from TravelingTony.TestCase                   import TestCase
from TravelingTony.Constants                  import TT_Constants
from TravelingTony.pages.ShareOnFacebookPage  import ShareOnFacebookPage
import unittest
import nose
from nose.plugins.attrib import attr


class ShareOnFacebookTest(TestCase, unittest.TestCase):

    def setUp(self):
        super(ShareOnFacebookTest, self).setUp()
      
    @attr(priority="low")  
    def test_ShareOnFacebookTest(self):
        share_on_facebook_page_obj = ShareOnFacebookPage(self.driver)
        share_on_facebook_page_obj.share()
    
    def tearDown(self):
        super(ShareOnFacebookTest, self).tearDown()
        

if __name__ == "__main__":
   nose.main()





```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
