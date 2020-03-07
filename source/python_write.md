---
title: python write (snippet)
date: 2019-02-07
tags: ["python"]
---

## python write

Python beginners example: python write

```python
# from sys module import a member called 'argv'
from sys import argv
#unpack
script, filename = argv
fp = open(filename, "w")
print("Writing to file %r " % fp)
fp.write("Hello World")
fp.close()


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
