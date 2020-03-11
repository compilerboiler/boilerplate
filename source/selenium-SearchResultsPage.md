---
title: selenium SearchResultsPage (snippet)
date: 2020-02-13
tags: ["python"]
---
Python web automation, selenium example 'SearchResultsPage'


## SearchResultsPage

Python selenium example: SearchResultsPage

```python
from BasePage                import BasePage
from TravelingTony.Constants import TT_Constants
from BasePage                import IncorrectPageException
from TravelingTony.UIMap     import SearchResultsPageMap


class SearchResultsPage(BasePage):

    def __init__(self, driver):
        super(SearchResultsPage, self).__init__(driver)
  

    def _verify_page(self):
        try:
          self.wait_for_element_visibility(10, 
                                         "xpath", 
                                         SearchResultsPageMap['ProductImagesXpath']
          )
        except:   
          raise IncorrectPageException
    
    
    
      
    



```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
