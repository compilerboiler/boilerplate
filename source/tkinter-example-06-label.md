---
title: tkinter example 06-label (snippet)
date: 2020-02-09
tags: ["python"]
---
Python tkinter (gui) example '06-label'


## 06-label

Python tkinter example: 06-label

```python
from tkinter import *

my_window = Tk() # crea un objeto por defecto

# CODE GOES HERE
my_window.title("Label introduction")

# Creamos label en nuestra ventana
label_1 = Label(my_window, text='This is label 1', background="blue", foreground="white")
label_2 = Label(my_window, text='This is label 2', bg='#7fff00', fg='black')
label_3 = Label(my_window,
                text='Blue text in Verdana 16 bolt italic Font',
                fg='blue',
                font='Verdana 16 bold italic')


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
