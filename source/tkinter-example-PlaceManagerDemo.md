---
title: tkinter example PlaceManagerDemo (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example 'PlaceManagerDemo'


## PlaceManagerDemo

Python tkinter example: PlaceManagerDemo

```python
from tkinter import * # Import tkinter
    
class PlaceManagerDemo:
    def __init__(self):
        window = Tk() # Create a window
        window.title("Place Manager Demo") # Set title
        
        Label(window, text = "Blue", bg = "blue").place(
            x = 20, y = 20)
        Label(window, text = "Red", bg = "red").place(
            x = 50, y = 50)
        Label(window, text = "Green", bg = "green").place(
            x = 80, y = 80)
        
        window.mainloop() # Create an event loop

PlaceManagerDemo() # Create GUI 

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
