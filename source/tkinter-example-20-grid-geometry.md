---
title: tkinter example 20-grid-geometry (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example '20-grid-geometry'


## 20-grid-geometry

Python tkinter example: 20-grid-geometry

```python
from tkinter import *

my_window = Tk()

label_1 = Label(my_window, width='20', height='3', bg='red')
label_2 = Label(my_window, width='20', height='3', bg='green')
label_3 = Label(my_window, width='20', height='3', bg='blue')
label_4 = Label(my_window, width='20', height='3', bg='white')
label_5 = Label(my_window, width='20', height='3', bg='black')
label_6 = Label(my_window, width='20', height='3', bg='grey')
label_7 = Label(my_window, width='20', height='3', bg='#4477af')
label_8 = Label(my_window, width='20', height='3', bg='#997755')
label_9 = Label(my_window, width='20', height='3', bg='#fabada')

label_1.grid(row=0, column=0)
label_2.grid(row=0, column=1)
label_3.grid(row=0, column=2)
label_4.grid(row=1, column=0)
label_5.grid(row=1, column=1)
label_6.grid(row=1, column=2)
label_7.grid(row=2, column=0)
label_8.grid(row=2, column=1)
label_9.grid(row=2, column=2)

# bucle principal
my_window.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
