---
title: tkinter example 17-stringvar-textvariable (snippet)
date: 2020-02-09
tags: ["python"]
---
Python tkinter (gui) example '17-stringvar-textvariable'


## 17-stringvar-textvariable

Python tkinter example: 17-stringvar-textvariable

```python
from tkinter import *

my_window = Tk() # crea un objeto por defecto

# CODE
var_1 = StringVar() # crea un string que se puede asociar con un Label

label_1 = Label(my_window,
                relief='solid',
                font='Times 22 bold',
                textvariable=var_1)

label_1.pack()
res = input('Mensaje: ')
var_1.set(res)

# bucle principal
my_window.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
