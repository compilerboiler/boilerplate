---
title: tkinter example 02-background (snippet)
date: 2020-02-09
tags: ["python"]
---
Python tkinter (gui) example '02-background'


## 02-background

Python tkinter example: 02-background

```python
"""
https://www.w3schools.com/colors/colors_picker.asp
"""

from tkinter import *

my_window = Tk() # crea un objeto por defecto: fondo gris, maximizar, minimizar, etc.

# CODE GOES HERE
my_window.title("Demo1")

# set the background of the window
# también se puede usar bg en vez de background
# Se puede usar número hexadecimal: '#00ff00' en vez de 'green'

# my_window.configure(background='green')
my_window.configure(background='#94d42b')

#bucle principal
my_window.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
