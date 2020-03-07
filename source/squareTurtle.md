---
title: squareTurtle (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'squareTurtle'

Functions in program: 
* `def square():`

Modules used in program: 
* `import turtle`

## squareTurtle

Python beginners example: squareTurtle

```python
import turtle

def square():
    win = turtle.Screen()
    win.bgcolor("white")
    jack = turtle.Turtle()
    for x in range(1,5):
              jack.forward(100)
              jack.right(90)
    win.exitonclick()
       
square()      


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
