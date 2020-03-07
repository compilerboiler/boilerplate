---
title: turtleRandomWeb (snippet)
date: 2019-02-07
tags: ["python"]
---

## turtleRandomWeb

Python beginners example: turtleRandomWeb

```python
import random
import turtle
t = turtle.Pen()

for i in range(150):
    t.color(random.choice(['green','red','violet']))
    t.width(5)
    t.forward(i)
    t.right(30)


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
