---
title: tkinter example 09-label-border (snippet)
date: 2020-02-09
tags: ["python"]
---
Python tkinter (gui) example '09-label-border'


## 09-label-border

Python tkinter example: 09-label-border

```python
from tkinter import *

my_window = Tk() # crea un objeto por defecto

# CODE GOES HERE
my_window.title("Label")

# Creamos label en nuestra ventana
# borderwidth = bd
label_1 = Label(my_window, text='Hello world', borderwidth=1, relief='solid', font='Times 12')
label_1.pack()
# se puede usar relief: solid, raised, sunken, ridge, groove, flat

# bucle principal
my_window.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
