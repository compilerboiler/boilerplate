---
title: tkinter example 26-entry-tab-focus (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example '26-entry-tab-focus'


## 26-entry-tab-focus

Python tkinter example: 26-entry-tab-focus

```python
from tkinter import *


my_window = Tk()

# build the GUI
entry_a = Entry(my_window, bg='red')
entry_b = Entry(my_window, bg='yellow')
entry_c = Entry(my_window, bg='white')

label_a = Label(my_window, text='First Name')
label_b = Label(my_window, text='Middle Name')
label_c = Label(my_window, text='Last Name')

entry_a.grid(row=0, column=1)
entry_b.grid(row=1, column=1)
entry_c.grid(row=2, column=1)

label_a.grid(row=0, column=0)
label_b.grid(row=1, column=0)
label_c.grid(row=2, column=0)

entry_a.focus()

my_window.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
