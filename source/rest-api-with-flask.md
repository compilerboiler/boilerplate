---
date: 2020-02-16
title: rest api with flask
---
The Python <a href="https://palletsprojects.com/p/flask/">Flask</a> module is great for building a Rest API. A Rest API uses the <a href="https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol">HTTP</a> protocol as it was originally designed. 

The HTTP protocol has many requests like **GET, PUT, POST, and DELETE** requests. These requests should be used for mutation, creation, and deletion respectively.

This is great for making your web app backend. Because it decouples your backend (logic) from your frontend (presentation). 

This means you can update your frontend without having to recode your backend all over again.

You can put <a href="https://pythonbasics.org/python-to-web/">your Python apps online</a> easily.


## Get request

A get request is the most basic. This is when you use your browser to open a url. The underlying HTTP protocol then does the GET request on which the server returns the data.

Lest return <a href="https://pythonprogramminglanguage.com/python-json/">JSON</a> data from our **Flask Rest API**, you can do that like this:

```python
from flask import Flask, jsonify, request

app = Flask(__name__)

incomes = [
  { 'name': 'Alice', 'amount': 2000 },
  { 'name': 'Abbey', 'amount': 2200 },
]

@app.route('/incomes')
def get_incomes():
  return jsonify(incomes)

app.run(host='0.0.0.0', port=8080)
```

Then open the url *localhost:8080/incomes* to see the JSON data presented. The front-end (Javascript) is great at parsing and creating JSON data.

![json data](https://dev-to-uploads.s3.amazonaws.com/i/emcxcqhlfamydf81vrjz.png)

## Post requests

Post requests are used to insert data. The user normally doesn't make a post request, the front-end does this. However, you can mimick this using a tool called `curl` or use an extension.

Add a new request for a post request

```python
@app.route('/incomes', methods=['POST'])
def add_income():
  incomes.append(request.get_json())
  return '', 204
```

Then you can make a post request. To make a post request, you can use curl.

    curl -X POST -H "Content-Type: application/json" -d '{"name":"Aaron","amount":5000}' http://localhost:8080/incomes 

Normally your web app will do the web request. If you don't feel comfortable with the terminal, you can use the postman extension.

![http post](https://dev-to-uploads.s3.amazonaws.com/i/rsxuuiw2u8ybjvcnakm6.png)

For an online app, you'll want to add authentication, input validation and a lot more. If you are new to Flask, I recommend this <a href="https://gumroad.com/l/IMzBy">Flask course</a>.
