---
title: simple UIMap (snippet)
date: 2020-02-12
tags: ["python"]
---
Python web automation, selenium example 'UIMap'


## UIMap

Python selenium example: UIMap

```python
ContactPageMap = dict(FirstNameFieldXpath  = "//input[contains(@name, 'first')]",
                      LastNameFieldXpath   = "//input[contains(@name, 'last')]",
                      EmailFieldXpath      = "(//input[contains(@id, 'input')])[3]",
                      CommentFieldXpath    = "//textarea",
                      SubmitButtonXpath    = "//span[.='Submit']",
                      ThankYouMessageXpath = "//div[contains(text(), 'Thank you')]"
)

FacebookLoginPageMap = dict(UsernameFieldID = "email",
                            PasswordFieldID = "pass",
                            LoginButtonName = "login"
)

ProductPageMap = dict(QuantityDropDownID     = "wsite-com-product-option-Quantity",
                      FacebookShareLinkXpath = "//a[@title='Share on Facebook']"
)

ShareOnFacebookPageMap = dict(ShareLinkButtonName = "share"
)


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
