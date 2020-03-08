---
title: tkinter example 28-object-oriented (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example '28-object-oriented'


## 28-object-oriented

Python tkinter example: 28-object-oriented

```python
from tkinter import *

# main window
my_window = Tk()

# build the GUI
button_a = Button(my_window, text='BUTTON A', relief= FLAT, bd=4).grid(row=0, column=0)
button_b = Button(my_window, text='BUTTON B', relief= RAISED, bd=4).grid(row=0, column=1)
button_c = Button(my_window, text='BUTTON C', relief= SUNKEN, bd=4).grid(row=0, column=2)
button_d = Button(my_window, text='BUTTON D', relief= GROOVE, bd=4).grid(row=1, column=0)
button_e = Button(my_window, text='BUTTON E', relief= RIDGE, bd=4).grid(row=1, column=1)

my_window.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
