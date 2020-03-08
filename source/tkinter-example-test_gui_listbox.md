---
title: tkinter example test gui listbox (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example 'test gui listbox'

Functions in program: 
* `def callback():`

## test gui listbox

Python tkinter example: test gui listbox

```python
from tkinter import *
from tkinter import messagebox

def callback():
    print("called the callback!")

root = Tk()

# create a menu
menu = Menu(root)
root.config(menu=menu)

filemenu = Menu(menu)
menu.add_cascade(label="File", menu=filemenu)
filemenu.add_command(label="New", command=callback)
filemenu.add_command(label="Open...", command=callback)
filemenu.add_separator()
filemenu.add_command(label="Exit", command=callback)

helpmenu = Menu(menu)
menu.add_cascade(label="Help", menu=helpmenu)
helpmenu.add_command(label="About...", command=callback)

"""
Lb1 = Listbox(root, selectmode=EXTENDED)

names = ["One", "Two", "Three", "Four", "Five"]
for i,name in enumerate(names):
    Lb1.insert(i, name)

Lb1.pack()
"""

mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
