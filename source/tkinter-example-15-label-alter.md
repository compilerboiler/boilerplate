---
title: tkinter example 15-label-alter (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example '15-label-alter'


## 15-label-alter

Python tkinter example: 15-label-alter

```python
from tkinter import *

my_window = Tk() # crea un objeto por defecto

# CODE
label_1 = Label(my_window,
                borderwidth=4,
                relief='solid',
                font='Times 22 bold',
                background='red',
                foreground='white',
                text='Hola Mundo')

label_1.pack()

# podemos acceder a los value a traves de su key como en cualquier diccionario
print(label_1['bd'])

# Modificamos las opciones, incluso de las que no existian
label_1['bg'] = 'blue'
label_1['text'] = 'Texto Cambiado'
label_1['padx'] = 20
# bucle principal
my_window.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
