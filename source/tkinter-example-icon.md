---
title: tkinter example icon (snippet)
date: 2020-02-09
tags: ["python"]
---
Python tkinter (gui) example 'icon'


## icon

Python tkinter example: icon

```python
from tkinter import *

root = Tk()

icon = PhotoImage(file="mario.png")
lbl = Label(root, text="Welcome", image=icon)
lbl.pack()

root.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
