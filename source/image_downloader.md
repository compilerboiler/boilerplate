---
title: image downloader (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'image downloader'

Functions in program: 
* def download_image(url):

Modules used in program: 
* import urllib.request
* import random

## image downloader

Python beginners example: image downloader

```python
import random
import urllib.request

get = str(input("Enter url of image to download :  "))

def download_image(url):
    name = random.randrange(1, 1000)
    full_name = str(name) + ".jpg"
    urllib.request.urlretrieve(url, full_name)

print(download_image(get))


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
- Another Python site: https://pythonprogramminglanguage.com
