---
title: tkinter example slider (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example 'slider'

Functions in program: 
* `def show_values():`

## slider

Python tkinter example: slider

```python
from tkinter import *


def show_values():
    print((w1.get(), w2.get()))

master = Tk()
w1 = Scale(master, from_=0, to=42, tickinterval=0)
w1.set(19)
w1.pack()
w2 = Scale(master, from_=0, to=200, length=600, tickinterval=10, orient=HORIZONTAL)
w2.set(23)
w2.pack()
Button(master, text='Show', command=show_values).pack()

mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
