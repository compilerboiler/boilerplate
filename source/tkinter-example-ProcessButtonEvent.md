---
title: tkinter example ProcessButtonEvent (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example 'ProcessButtonEvent'

Functions in program: 
* `def processCancel():`
* `def processOK():`

## ProcessButtonEvent

Python tkinter example: ProcessButtonEvent

```python
from tkinter import * # Import tkinter

def processOK():
    print("OK button is clicked")
 
def processCancel():
    print("Cancel button is clicked")
    
root = Tk() # Create a root window
btOK = Button(root, text = "OK", fg = "red", command = processOK) 
btCancel = Button(root, text = "Cancel", bg = "yellow", 
                  command = processCancel) 
btOK.pack() # Place the button in the window
btCancel.pack() # Place the button in the window

root.mainloop() # Create an event loop

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
