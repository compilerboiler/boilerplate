---
title: tkinter example GridManagerDemo (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example 'GridManagerDemo'


## GridManagerDemo

Python tkinter example: GridManagerDemo

```python
from tkinter import * # Import tkinter
    
class GridManagerDemo:
    window = Tk() # Create a window
    window.title("Grid Manager Demo") # Set title
    
    message = Message(window, text = 
        "This Message widget occupies three rows and two columns")
    message.grid(row = 1, column = 1, rowspan = 3, columnspan = 2)
    Label(window, text = "First Name:").grid(row = 1, column = 3)
    Entry(window).grid(row = 1, column = 4, padx = 5, pady = 5)
    Label(window, text = "Last Name:").grid(row = 2, column = 3)
    Entry(window).grid(row = 2, column = 4)
    Button(window, text = "Get Name").grid(row = 3, 
        padx = 5, pady = 5, column = 4, sticky = E)
    
    window.mainloop() # Create an event loop

GridManagerDemo() # Create GUI 

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
