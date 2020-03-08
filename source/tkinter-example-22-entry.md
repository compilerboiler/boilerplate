---
title: tkinter example 22-entry (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example '22-entry'

Functions in program: 
* `def salute():`

## 22-entry

Python tkinter example: 22-entry

```python
from tkinter import *

def salute():
    name = entry_1.get()
    message = 'Hola {}'.format(name)
    label_2['text'] = message

my_window = Tk()

label_1 = Label(my_window, text='¿Cómo te llamas?')
entry_1 = Entry(my_window)
button_1 = Button(my_window, text='Salute', command=salute)
label_2 = Label(my_window)

label_1.grid(row=0, column=0)
entry_1.grid(row=0, column=1)
button_1.grid(row=1, column=0)
label_2.grid(row=1, column=1)

my_window.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
