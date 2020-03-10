---
title: simple python-example-78 (snippet)
date: 2020-02-10
tags: ["python"]
---
Python example 'python-example-78'


## python-example-78

Python example: python-example-78

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

if __name__ == '__main__':
    person = {"li":18,"wang":50,"zhang":20,"sun":22}
    m = 'li'
    for key in person.keys():
        if person[m] < person[key]:
            m = key

    print('%s,%d' % (m,person[m]))


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
