---
title: tkinter example 12-space-around-label (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example '12-space-around-label'


## 12-space-around-label

Python tkinter example: 12-space-around-label

```python
from tkinter import *

my_window = Tk() # crea un objeto por defecto

# CODE GOES HERE
my_window.title("Label")
my_window.geometry('400x250')

# Creamos label en nuestra ventana
label_1 = Label(my_window,
                 text='spacer')
label_2 = Label(my_window,
                text='Hello World',
                borderwidth=1,
                relief='solid',
                font='Times 32')
label_3 = Label(my_window,
                 text='spacer')
label_4 = Label(my_window,
                text='Hello World',
                borderwidth=1,
                relief='solid',
                font='Times 32',
                padx=80,    # padx añade padding horizontal a ambos lados
                pady=20)    # pady similar pero vertical

label_1.pack()
label_2.pack()
label_3.pack()
label_4.pack()

# bucle principal
my_window.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
