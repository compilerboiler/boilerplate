---
title: mod example (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'mod example'

Functions in program: 
* `def downloadImage(url):`

Modules used in program: 
* `import urllib.request`
* `import random`

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
