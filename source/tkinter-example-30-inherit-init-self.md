---
title: tkinter example 30-inherit-init-self (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example '30-inherit-init-self'


## 30-inherit-init-self

Python tkinter example: 30-inherit-init-self

```python
from tkinter import *

class TipicalFrame(Frame):
    def __init__(self, the_window, **kwargs):
        super().__init__(**kwargs)
        self['height']=150
        self['width']=150
        self['bd']=8
        print('id of self is {}'.format(id(self)))


# main window
my_window = Tk()

# build the GUI
frame_a = TipicalFrame(my_window, relief=RAISED, bg='red')
print('id of frame_a is {}'.format(id(frame_a)))

frame_b = TipicalFrame(my_window, relief=SUNKEN, bg='green')
print('id of frame_b is {}'.format(id(frame_b)))


frame_a.grid(row=0, column=0)
frame_b.grid(row=0, column=1)

my_window.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
