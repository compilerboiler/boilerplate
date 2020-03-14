---
date: 2020-02-16
title: web app with python
---
---
tags: ["python"]
date: 2020-02-16
title: web app with python
---
---
tags: ["python"]
date: 2020-02-14
title: web app with python
---
You can do web development in Python. Make a web app or website with <a href="https://python.org">Python</a>? It's easier than you think.

First pick a web development module. There are many like 

* <a href="https://palletsprojects.com/p/flask/">Flask</a>
* <a href="https://www.djangoproject.com/">Django</a>
* <a href="https://twistedmatrix.com/trac/wiki/Documentation">Twisted</a> 
* <a href="https://bottlepy.org/">Bottle</a>
* and others.

Install the module and learn how to use it. There are a lot of modules and they all are a bit different. 

Flask is the most commonly used. Django is also popular, but it's learning curve can be challenging.

Putting <a href="https://pythonbasics.org/python-to-web/">your python app on the web</a> is easy, even no need to maintain servers.

## Hello world demo (Twisted)

To get started with building your app, it's recommended that you use a virtual environment. This prevents package conflicts on your system. 

First setup your <a href="https://pythonbasics.org/virtualenv/">virtual environment</a> and then install one of the many Python web modules.

For this article I'll go with `twisted`

    pip3 install twisted

Twisted can be used to make web apps, but it supports many other network protocols like SMTP, POP3, IMAP, SSHv2, and DNS. 

Create your program, app.py

```python
from twisted.web import server, resource
from twisted.internet import reactor, endpoints

class Counter(resource.Resource):
    isLeaf = True
    numberRequests = 0

    def render_GET(self, request):
        self.numberRequests += 1
        request.setHeader(b"content-type", b"text/plain")
        content = u"Hello World #{}\n".format(self.numberRequests)
        return content.encode("ascii")

endpoints.serverFromString(reactor, "tcp:8080").listen(server.Site(Counter()))
reactor.run()
```

Then open localhost at port 8080 and you'll see the hello world message:

![hello world in twisted](https://dev-to-uploads.s3.amazonaws.com/i/3b4pgki93o1lvhz3tf56.png)

If you want to have your app online instead, you can follow <a href="https://pythonbasics.org/python-to-web/">this guide</a>

## Hello world demo (Flask)

If you want to use Flask instead, you can use the code below. It starts the server at port 8080 and will do exactly the same.

The difference between Twisted and Flask is, that Flask is designed for web apps only. It supports many things you may need like Templates and URL routing out of the box.

```python
from flask import Flask

app = Flask(__name__)

@app.route('/')
def index():
    return 'Hello world'

app.run(host='0.0.0.0', port=8080)
```

Open the browser at that url, and you'll see "hello world" appear. If you are new to Flask, this is a good <a href="https://gumroad.com/l/IMzBy">Flask course</a>.

## Hello world in Bottle

Bottle is a simple WSGI micro web-framework for Python. It doesn't have any dependencies other than the Python Standard Library.

It has these features:

* Routing: map URLs to function
* Templates: template engine and support for mako, jinja2 and cheetah templates.
* Utilities: Convenient access to form data, file uploads, cookies, headers and other HTTP-related metadata.
* Server: Built-in HTTP development server and support for paste, fapws3, bjoern, gae, cherrypy or any other WSGI capable HTTP server.


```python
from bottle import route, run

@route('/hello')
def hello():
    return "Hello World!"

run(host='localhost', port=8080, debug=True)
```

Then open localhost:8080 and url `/hello` (there is a url route). See the decorator

```python
@route('/hello')
```

that maps the url to the function

```python
def hello():
    return "Hello World!"
```

Personally I don't think the Bottle framework offers any advantages over the Flask framework, while Flask offers many advantages over Bottle. In short, go with Flask. Bottle is for tiny projects.


