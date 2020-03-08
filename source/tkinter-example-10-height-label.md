---
title: tkinter example 10-height-label (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example '10-height-label'


## 10-height-label

Python tkinter example: 10-height-label

```python
from tkinter import *

my_window = Tk() # crea un objeto por defecto

# CODE GOES HERE
my_window.title("Label")

# Creamos label en nuestra ventana
# borderwidth = bd
label_1 = Label(my_window,
                text='Line1\nLine 2',
                borderwidth=1,
                relief='solid',
                font='Times 12',
                height=2)
label_1.pack()
# se puede usar relief: solid, raised, sunken, ridge, groove, flat

# bucle principal
my_window.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
