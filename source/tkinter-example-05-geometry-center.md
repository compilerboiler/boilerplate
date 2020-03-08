---
title: tkinter example 05-geometry-center (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example '05-geometry-center'


## 05-geometry-center

Python tkinter example: 05-geometry-center

```python
from tkinter import *

my_window = Tk() # crea un objeto por defecto: fondo gris, maximizar, minimizar, etc.

# CODE GOES HERE
my_window.title("Ventana en centro de pantalla")

# window size
width_of_window = 400
heigth_of_window = 200

# screen size
screen_width = my_window.winfo_screenwidth()
screen_heigth = my_window.winfo_screenheight()

# coordinate por (x,y) NW window position
x_coordinate = int((screen_width/2) - (width_of_window/2))
y_coordinate = int((screen_heigth/2) - (heigth_of_window/2))

# geometry
my_window.geometry('{}x{}+{}+{}'.format(width_of_window,
                                        heigth_of_window,
                                        x_coordinate,
                                        y_coordinate))

# bucle principal
my_window.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
