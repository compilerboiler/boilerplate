---
title: tkinter example 07-label-width (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example '07-label-width'


## 07-label-width

Python tkinter example: 07-label-width

```python
from tkinter import *

my_window = Tk() # crea un objeto por defecto

# CODE GOES HERE
my_window.title("Label introduction")

# Creamos label en nuestra ventana
# el ancho (widht) va en funcioón del tamaño de la fuente y no de los píxeles
label_1 = Label(my_window, text='This is label 1', background="red", font='Times 12', width=20)
label_2 = Label(my_window, text='This is label 2', bg='#7fff00', font='Times 12', width=30)
label_3 = Label(my_window, text='This is label 3', bg='blue', font='Times 12', width=40)


# el orden en que aparecen labels en al ventana dependen del orden en que usemos pack()
label_1.pack() # la ventana se redimensiona para que quepa el texto completo
label_2.pack()
label_3.pack()

# bucle principal
my_window.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
