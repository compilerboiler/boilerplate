---
title: tkinter example 04-geometry (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example '04-geometry'


## 04-geometry

Python tkinter example: 04-geometry

```python
from tkinter import *

my_window = Tk() # crea un objeto por defecto: fondo gris, maximizar, minimizar, etc.

# CODE GOES HERE
my_window.title("Demo1")

# my_window.geometry('width'x'heith'+'x_position'+'y_position')
my_window.geometry("400x200+500+50")
# modificaciones del tamaño de la ventana
my_window.resizable(width=False, height=True)

#bucle principal
my_window.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
