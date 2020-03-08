---
title: tkinter example panedWindow (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example 'panedWindow'


## panedWindow

Python tkinter example: panedWindow

```python
from tkinter import *

root = Tk()

m1 = PanedWindow()
m1.pack(fill=BOTH, expand=1)

left = Label(m1, text="left pane")
m1.add(left)

m2 = PanedWindow(m1, orient=VERTICAL)
m1.add(m2)

top = Label(m2, text="top pane")
m2.add(top)

bottom = Label(m2, text="bottom pane")

m2.add(bottom)

root.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
