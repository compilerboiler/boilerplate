---
title: selenium Example22AssertInAndNotIn (snippet)
date: 2020-02-13
tags: ["python"]
---
Python web automation, selenium example 'Example22AssertInAndNotIn'


Modules used in program: 
* `import unittest`

## Example22AssertInAndNotIn

Python selenium example: Example22AssertInAndNotIn

```python
import unittest


class Test(unittest.TestCase):
    def testName(self):
        my_list = {"python", "selenium", "java"}
        self.assertIn("python", my_list)
        self.assertNotIn("JavaScript", my_list)


if __name__ == "__main__":
    unittest.main()


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
