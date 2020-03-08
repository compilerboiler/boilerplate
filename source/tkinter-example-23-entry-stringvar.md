---
title: tkinter example 23-entry-stringvar (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example '23-entry-stringvar'

Functions in program: 
* `def salute():`

## 23-entry-stringvar

Python tkinter example: 23-entry-stringvar

```python
from tkinter import *

def salute():
    """ modify lable_2's saludo """
    var_saludo.set('Hola ' + var_name.get()) # modificamos var_1

# variables
my_window = Tk()
var_saludo = StringVar()
var_name = StringVar()

# build the GUI
label_1 = Label(my_window, text='¿Cómo te llamas?')
entry_1 = Entry(my_window, textvariable=var_name)
button_1 = Button(my_window, text='Salute', command=salute)
label_2 = Label(my_window, textvariable=var_saludo)

label_1.grid(row=0, column=0)
entry_1.grid(row=0, column=1)
button_1.grid(row=1, column=0)
label_2.grid(row=1, column=1)

my_window.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
