---
title: tkinter example PackManagerDemoWithSide (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example 'PackManagerDemoWithSide'


## PackManagerDemoWithSide

Python tkinter example: PackManagerDemoWithSide

```python
from tkinter import * # Import tkinter
    
class PackManagerDemoWithSide:
    window = Tk() # Create a window
    window.title("Pack Manager Demo 2") # Set title
    
    Label(window, text = "Blue", bg = "blue").pack(side = LEFT)
    Label(window, text = "Red", bg = "red").pack(
        side = LEFT, fill = BOTH, expand = 1)
    Label(window, text = "Green", bg = "green").pack(
        side = LEFT, fill = BOTH)
    
    window.mainloop() # Create an event loop
        
PackManagerDemoWithSide() # Create GUI 

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
