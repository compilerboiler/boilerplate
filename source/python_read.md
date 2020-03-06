---
title: python read
date: 2019-02-07
---

## python read

Python beginners example: python read

```python
# from sys module import a member called 'argv'
from sys import argv
#unpack
script, filename = argv
fp = open(filename)
print("Reading file %r " % fp)
print(fp.read())
fp.close()


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
