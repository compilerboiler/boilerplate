---
title: tkinter example tictoetic (snippet)
date: 2020-02-09
tags: ["python"]
---
Python tkinter (gui) example 'tictoetic'


## tictoetic

Python tkinter example: tictoetic

```python
from tkinter import * # Import tkinter
from random import randint

class MainGUI:
    def __init__(self):
        window = Tk() # Create a window
        window.title("TicTacToe") # Set a title
        
        imageX = PhotoImage(file = "image/x.gif")
        imageO = PhotoImage(file = "image/o.gif")
        
        for i in range(3):
            frame = Frame(window)
            frame.pack()
            for j in range(3):
                label = Label(frame, image = imageX if randint(0, 1) == 0 else imageO )
                label.pack(side = LEFT)
        
        window.mainloop() # Create an event loop

MainGUI()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
