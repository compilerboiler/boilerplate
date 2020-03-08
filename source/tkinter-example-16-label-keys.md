---
title: tkinter example 16-label-keys (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example '16-label-keys'


## 16-label-keys

Python tkinter example: 16-label-keys

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
print(label_1.keys())

for item in label_1.keys():
    print('{}: {}'.format(item, label_1[item]))
# bucle principal
my_window.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
