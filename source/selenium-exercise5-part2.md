---
title: simple exercise5-part2 (snippet)
date: 2020-02-12
tags: ["python"]
---
Python web automation, selenium example 'exercise5-part2'


Modules used in program: 
* `import time`
* `import unittest`

## exercise5-part2

Python selenium example: exercise5-part2

```python
from TravelingTony.TestCase                   import TestCase
from TravelingTony.Constants                  import TT_Constants
from TravelingTony.Common                     import Common
import unittest
import time

class ShareOnTwitterTest(TestCase, unittest.TestCase):

    def setUp(self):
        super(ShareOnTwitterTest, self).setUp()
        
        
    def test_ShareOnTwitterTest(self):
        common_obj = Common(self.driver)
        # All we have to do here is click the "Tweet" button. We locate this button by value using Css Selector.
        common_obj.click(10, "cssSelector", "input[value=Tweet]")
        """
        Just using time.sleep() so that you see the last webdriver action.
        I do not recommend using this in your tests.
        """
        time.sleep(5)
    
    def tearDown(self):
        super(ShareOnTwitterTest, self).tearDown()
        

if __name__ == "__main__":
   unittest.main()





```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
