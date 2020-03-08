---
title: tkinter example 18-stringvar-set (snippet)
date: 2020-02-09
tags: ["python"]
---
Python tkinter (gui) example '18-stringvar-set'


## 18-stringvar-set

Python tkinter example: 18-stringvar-set

```python
from tkinter import *

my_window = Tk() # crea un objeto por defecto

# CODE
var_1 = StringVar() # crea un string que se puede asociar con un Label

label_1 = Label(my_window,
                relief='solid',
                font='Times 22 bold')
label_2 = Label(my_window,
                relief='solid',
                font='Times 22 bold',
                textvariable=var_1)

label_1.pack()
label_2.pack()
label_1['text'] = 'Usando key/value'
var_1.set('Usando textvariable y StringVar()')

# bucle principal
my_window.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
