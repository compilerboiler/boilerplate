---
title: tkinter example conv (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example 'conv'

Functions in program: 
* `def calculate(*args):`

## conv

Python tkinter example: conv

```python
from Tkinter import *
def calculate(*args):
    try:
        value = float(feet.get())
        meters.set((0.3048 * value * 10000.0 + 0.5)/10000.0)
    except ValueError:
        pass

root = Tk()
root.title("Feet to Meters")
mainframe = Frame(root, padx=3,pady=12)
mainframe.grid(column=0, row=0, sticky=(N, W, E, S))
mainframe.columnconfigure(0, weight=1)
mainframe.rowconfigure(0, weight=1)

feet = StringVar()
meters = StringVar()
feet_entry = Entry(mainframe, width=7, textvariable=feet)
feet_entry.grid(column=2, row=1, sticky=(W, E))
Label(mainframe, textvariable=meters).grid(column=2, row=2, sticky=(W, E))
Button(mainframe, text="Calculate", command=calculate).grid(column=3, row=3, sticky=W)
Label(mainframe, text="feet").grid(column=3, row=1, sticky=W)
Label(mainframe, text="is equivalent to").grid(column=1, row=2, sticky=E)
Label(mainframe, text="meters").grid(column=3, row=2, sticky=W)

for child in mainframe.winfo_children(): child.grid_configure(padx=5, pady=5)
feet_entry.focus()
root.bind('<Return>', calculate)
root.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter