---
title: selenium WelcomePage (snippet)
date: 2020-02-13
tags: ["python"]
---
Python web automation, selenium example 'WelcomePage'


## WelcomePage

Python selenium example: WelcomePage

```python
from BasePage                import BasePage
from SearchResultsPage       import SearchResultsPage
from TravelingTony.Constants import TT_Constants
from BasePage                import IncorrectPageException
from TravelingTony.UIMap     import WelcomePageMap

class WelcomePage(BasePage):

    def __init__(self, driver):
        super(WelcomePage, self).__init__(driver)
  

    def _verify_page(self):
        try:
          self.wait_for_element_visibility(10, 
                                         "xpath", 
                                         WelcomePageMap['SeeCoolestPhotosButtonXpath']
          )
        except:   
          raise IncorrectPageException
    
    def search(self, searchString):
        self.fill_out_field("name",
                            WelcomePageMap['SearchFieldName'],
                            searchString
        )
        self.click(10, 
                   "xpath", 
                   WelcomePageMap['SearchSubmitButtonXpath']
        )
        return SearchResultsPage(self.driver)
        
        
    
      
    



```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
