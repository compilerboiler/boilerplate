---
title: tkinter example 19-button-intro (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example '19-button-intro'

Functions in program: 
* `def add_label():`

## 19-button-intro

Python tkinter example: 19-button-intro

```python
from tkinter import *

def add_label():
    lable_1 = Label(my_window,
                    text='Botón pulsado')
    lable_1.pack()

my_window = Tk() # crea un objeto por defecto
my_window.geometry('200x100')

button_1 = Button(my_window,
                  relief='solid',
                  font='Times 22 bold',
                  text='Clic Me',
                  command=add_label)    # nombre de la función, sin invocar
                                        # sin paréntesis

button_1.pack()

# bucle principal
my_window.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
