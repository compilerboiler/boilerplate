---
title: tkinter example 11-text-positon (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example '11-text-positon'


## 11-text-positon

Python tkinter example: 11-text-positon

```python
from tkinter import *

my_window = Tk() # crea un objeto por defecto

# CODE GOES HERE
my_window.title("Label")
my_window.geometry('400x250')

# Creamos label en nuestra ventana
label_1 =  Label(my_window,
                 text='scacer')
label_2 = Label(my_window,
                text='Hello World\nHello World',
                borderwidth=1,
                relief='solid',
                font='Times 32',
                width=15,
                height=4,
                anchor=SW)
label_1.pack()
label_2.pack()
# se puede usar relief: solid, raised, sunken, ridge, groove, flat

# bucle principal
my_window.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
