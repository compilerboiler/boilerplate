---
date: 2020-02-16
title: flask jinja
---
---
tags: ["python"]
date: 2020-02-16
title: flask jinja
---
---
tags: ["python"]
date: 2020-02-14
title: flask jinja
---
You can build web applications in the <a href="https://python.org">Python</a> programming language with the <a href="https://palletsprojects.com/p/flask/">Flask framework</a> (<a href="https://pythonbasics.org/what-is-flask-python/">what is Flask</a>).

When creating the user interface, you want to use variables from your Python code. You can do that with a template engine. Templates are what the end user see in their web browser. 

That means that in Python code you have some output (variables), which are then passed to the template for that URL.

![template engine](https://dev-to-uploads.s3.amazonaws.com/i/pqii4yghm0hkd266tffu.png)

## What is Jinja

Jinja is the <a href="https://en.wikipedia.org/wiki/Comparison_of_web_template_engines">template engine</a> used by Flask. Every <a href="https://pythonbasics.org/flask-tutorial-templates/">Jinja</a> file is an <a href="https://en.wikipedia.org/wiki/HTML">HTML</a> file with a minor twist. 

Jinja templates use `{% ... %}` for expressions and logic, for outputting results while `{{ ... }}` is used. That means that the html is replace with values from your Python code.

So your jinja html file could look something like this:

```html
<head>
    <title>Jinja example</title>
</head>
<body>
    <h1>Chapter {{chapter}}</h1>
    <p>String a is {{a}}</p>
    <p>String b is {{b}}</p>
</body>
```

If you don't know Python, you should <a href="https://pythonbasics.org">learn Python</a> before trying Flask or playing with jinja.

## Quick examples

You can test the jinja2 template engine in the Python shell. First install Flask using the Python package manager <a href="https://pythonbasics.org/how-to-use-pip-and-pypi/">pip</a>. Then install it with

    pip install flask

Open up your Python shell to try out jinja:

```python
>>> from jinja2 import Template
>>> x = 3
>>> t = Template("Variable x is {{ x }}")
>>> t.render(x=x)
'Variable x is 3'
>>>
```

```python
>>> t = Template("Lucky numbers {% for i in range(1,10) %}{{ i }} " " {% endfor %}")
>>> t.render()
'Lucky numbers 1  2  3  4  5  6  7  8  9  '
>>> 
```

## Return templates

Import the require modules in Python

```python
from flask import Flask, render_template
```

In your Flask app you can return a jinja template. Create a new program (example.py) like this. It will render the jinja template ("template.html") and pass two variables a and b.

```python
from flask import Flask, render_template
app = Flask(__name__)


@app.route("/")
def template_test():
    return render_template('template.html', a="Hastalavista!", b=[1,2,3])


if __name__ == '__main__':
    app.run(debug=True)

```

Create a new directory named "templates". Inside that directory create a new file named "template.html" (see reference in code above).

You can write a complete html file, but this basic jinja template will suffice:

```html
<p>String a is {{a}}</p>
<p>Loop through variable b</p>
<ul>
{% for x in b %}
    <li>{{x}}</li> 
{% endfor %}
</ul>
```

![jinja](https://dev-to-uploads.s3.amazonaws.com/i/0im4efe091hugc6ql3in.png)
 
Run your program and open the url:

```
➜  python3 example.py
 * Serving Flask app "example" (lazy loading)
 * Environment: production
   WARNING: This is a development server. Do not use it in a production deployment.
   Use a production WSGI server instead.
 * Debug mode: on
 * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
 * Restarting with stat
 * Debugger is active!
 * Debugger PIN: 251-419-329
```

**Related links:**
* <a href="https://palletsprojects.com/p/flask/">Python Flask Web Framework official site</a>
* <a href="https://gumroad.com/l/IMzBy">Create Web Apps with Flask</a>

