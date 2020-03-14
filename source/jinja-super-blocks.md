---
date: 2020-02-16
title: jinja super blocks
---
---
tags: ["python"]
date: 2020-02-16
title: jinja super blocks
---
---
tags: ["python"]
date: 2020-02-14
title: jinja super blocks
---
In <a href="https://palletsprojects.com/p/jinja/">Jinja</a>, the template engine of <a href="https://palletsprojects.com/p/flask/">Flask</a> web framework (<a href="https://pythonbasics.org/what-is-flask-python/">what is Flask</a>?), you can create templates. You can use these templates to improve the user experience and pass Python data to the web browser.

But with a large app, you'd have to rewrite the same template over and over to get the same design?

Not exactly, there is a trick you can use to prevent you from repeating the same template code over and over.

<img src="https://dev-to-uploads.s3.amazonaws.com/i/cytuiju4nip16yg7mpgy.png" width="50%" alt="trick">

Before playing with Flask, you should know the <a href="https://pythonbasics.org">basics of Python</a>. If you don't know how to use templates yet, see <a href="https://dev.to/bluepaperbirds/jinja-299k">this post</a>

## Super blocks

So you want to add a design for all pages in your app?

Instead of copying and pasting the same code throughout all your files, you can use a super block.

There is an easier way, instead you can use a <a href="http://jinja.pocoo.org/docs/templates/#super-blocks">super block</a>. 

```python
{{ super() }}
```

We'll create a new file called layout.html in the directory templates. This is not a plain html file, but a <a href="https://pythonbasics.org/flask-tutorial-templates/">jinja</a> template. This is the contents of the file,

```html
<!DOCTYPE html>
  <head>
    <title>Flask Template Example</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="http://netdna.bootstrapcdn.com/bootstrap/3.0.0/css/bootstrap.min.css" rel="stylesheet" media="screen">
    <style type="text/css">
      .container {
        max-width: 500px;
        padding-top: 100px;
      }
      h2 {color: red;}
    </style>
  </head>
  <body>
    <div class="container">
      <h2>My App</h2>
      <br>
      {% block content %}{% endblock %}
      <br>
      <div class="footer">
        {% block footer %}
          The footer of the page
          <br>
          <br>
          <br>
        {% endblock %}
      </div>
    </div>
  </body>
</html>
```

Key here is the user of `{% block content %}` and `{% block footer %}`, which will inject your pages.

Then change template.html to have the surrounding tags:

```python
{% extends "layout.html" %}
{% block content %}
<p>String a is {{a}}</p>
<p>Loop through variable b</p>
<ul>
{% for x in b %}
    <li>{{x}}</li>
{% endfor %}
</ul>
{% endblock %}
```

It then surrounds your page with the design:

![flask use of layout](https://dev-to-uploads.s3.amazonaws.com/i/5hnqmeqqyngdsfqktk4o.png)

Start the server and open the url

```bash
$ python3 example.py
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

You can now apply this template to any URL route in your Flask app!


**Related links:**
* <a href="https://palletsprojects.com/p/flask/">Python Flask Web Framework official site</a>
* <a href="https://gumroad.com/l/IMzBy">Create Web Apps with Flask</a>

