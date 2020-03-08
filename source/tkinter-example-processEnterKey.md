---
title: tkinter example processEnterKey (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example 'processEnterKey'

Functions in program: 
* `def evaluate(event):`

## processEnterKey

Python tkinter example: processEnterKey

```python
from tkinter import *
from math import *

def evaluate(event):
    res.configure(text = "Result: " + str(eval(entry.get())))

w = Tk()
Label(w, text="Your Expression:").pack()
entry = Entry(w)
entry.bind("<Return>", evaluate)
entry.pack()
res = Label(w)
res.pack()
w.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
