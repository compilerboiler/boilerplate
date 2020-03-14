---
tags: ["python"]
date: 2020-02-16
title: return variables with flask
---
---
tags: ["python"]
date: 2020-02-14
title: return variables with flask
---
<a href="https://python.org">Python</a> can be used for web development, Flask is a Python web framework based on WSGI. Flask lets you build web apps with Python (<a href="https://pythonbasics.org/what-is-flask-python/">what is Flask</a>). 

You can use Flask to build single page apps, a blog, web apps and many more things. Some people use it to build a user interface on their <a href="https://raspberrypi.org/">Raspberry Pi</a>. 

Before playing with Flask, you should <a href="https://pythonbasics.org">learn Python</a>

## Return variables in Flask

There are different ways to return variables with Flask. Did you know you can use <a href="https://github.com/bluepaperbirds/f-Strings-examples">f-Strings</a> inside Flask?  This is one of the most simple ways.

If you want to return some variables for your request, you can do:

```python
return f'a is {a} and b is {b}'
```

So a full example of returning these two variables would be

```python
from flask import Flask

app = Flask(__name__)

@app.route('/')
def index():
    a = 62
    b = 41
    return f'a is {a} and b is {b}'

app.run(host='0.0.0.0', port=5000)
```

In the browser:

![flask variables](https://dev-to-uploads.s3.amazonaws.com/i/cmmm8tfdrcp7eynvoxi7.png)

Run the server and open the localhost url on your pc:

```
➜  ~ python3 example.py
 * Serving Flask app "example" (lazy loading)
 * Environment: production
   WARNING: This is a development server. Do not use it in a production deployment.
   Use a production WSGI server instead.
 * Debug mode: off
 * Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)
```

**Related links:**
* <a href="https://palletsprojects.com/p/flask/">Flask web application framework</a>
* <a href="https://pythonbasics.org/flask-tutorial-hello-world/">Flask tutorial</a>
