---
title: mod example (snippet)
date: 2019-02-07
tags: ["python"]
---

## mod example

Python beginners example: mod example

```python
import random
import urllib.request

def downloadImage(url):
    filename = str(random.randrange(1,1000))
    download = urllib.request.urlretrieve(url, filename)

downloadImage()



```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
