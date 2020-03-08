---
title: tkinter example argsInButtonCallback (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example 'argsInButtonCallback'

Functions in program: 
* `def make_callback(number):`
* `def callback(number):`

## argsInButtonCallback

Python tkinter example: argsInButtonCallback

```python
from tkinter import *

master = Tk()


def callback(number):
    print(number)


def make_callback(number):
    return (lambda: callback(number))


for i in range(0, 10):
    b = Button(master, text=str(i), command=make_callback(i))
    b.pack()

mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
