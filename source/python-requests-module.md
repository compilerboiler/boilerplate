---
tags: ["python"]
date: 2020-02-14
title: python requests module
---
The requests module lets you make HTTP requests in <a href="https://python.org">Python</a>. <a href="https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol">HTTP</a> is the protocol of the web. The HTTP protocol has different type of requests, like the get request.

## Examples

So how to use the HTTP protocol directly in Python? Here are some examples. As the name indicates, the GET requests received data from a website:

```python
>>> import requests
>>> requests.get('https://youtube.com')
<Response [200]>
>>> 
```

It returns a response. The HTTP protocol has many predefined responses:

* A response of 200 means it has successfully received the data. 
* The response 404 means the data is not found. 

You can store the output of the get function like this:

```python
>>> response = requests.get('https://youtube.com')
>>> response.status_code
200
>>> 
```

To get the content you can use this:

```python
>>> response.content
```

## Parsing data

All content is in <a href="https://en.wikipedia.org/wiki/HTML">HTML</a> format and maybe some JavaScript. This means that by eye it's hard to read, but a web browser converts HTML to what you see on the screen. 

You can <a href="https://pythonspot.com/http-parse-html-and-xhtml/">parse HTML</a> in Python, but if you need a web browser there are pre-made components you can use.

Data on the web is not always HTML either, sometimes you'll load an image or text file. 

Sometimes the data is in <a href="https://pythonbasics.org/json/">JSON format</a>, in that case you want to use the json module. JSON is often used on the web, its a format that lets you define objects. These objects can be converted to Python object and from Python objects to JSON.

You can get more data on the request here:

```
>>> response.headers
```

This gives many variables like format, cookies, content encoding etc.

## Download files

If you don't want to parse data, but just download it, you have several options.

You can use the requests module. The example below downloads an image file using requests.

```python
import requests
import shutil

image_url = "https://cdn.pixabay.com/photo/2020/01/31/19/21/ural-owl-4808774__340.jpg"
resp = requests.get(image_url, stream=True)
local_file = open('image.jpg', 'wb')
resp.raw.decode_content = True
shutil.copyfileobj(resp.raw, local_file)
```

To download files, you can use <a href="https://pythonprogramminglanguage.com/download-file/">urllib2</a>.

Its possible to use system tools too (wget, curl).

**Related links:**
* <a href="https://2.python-requests.org/en/master/">Requests module for Python</a>
* <a href="https://pythonbasics.org/">Learn Python</a>


