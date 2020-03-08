---
title: tkinter example 21-exercise (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example '21-exercise'

Functions in program: 
* `def set_blue():`
* `def set_green():`
* `def set_red():`

## 21-exercise

Python tkinter example: 21-exercise

```python
"""
https://www.youtube.com/watch?v=XZ2G29ZUaII&index=27&list=PL6lxxT7IdTxGoHfouzEK-dFcwr_QClME_

Produce a GUI using python an tkinter thas has three buttons and a label. Arrange for the clicking of a button
to set the background colour of the label to red, gren and blue

i.e. clicking one button changes the bakcground of the label to red, clicking the second button changes it to
green and clicking the third button changes it to blue.

Whe the program furst runs have the background of the label set at white. Have nothing displayed in the label
and have the text of the buttons display Red, Gren an Blue respectively.
"""
from tkinter import *

def set_red():
    label_1['bg']='red'

def set_green():
    label_1['bg']='green'

def set_blue():
    label_1['bg']='blue'

my_window = Tk()

label_1 = Label(my_window, width='20', height='3', background='white')
button_red = Button(my_window, text='Red', width=6, command=set_red)
button_green = Button(my_window, text='Green', width=6, command=set_green)
button_blue = Button(my_window, text='Blue', width=6, command=set_blue)

label_1.grid(row=0, column=1)
button_red.grid(row=1, column=0)
button_green.grid(row=1, column=1)
button_blue.grid(row=1, column=2)

my_window.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
