---
title: tkinter example inside the circle (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example 'inside the circle'

Functions in program: 
* `def distance(xCenter, yCenter, x, y):`
* `def isInsideCircle(xCenter, yCenter, radius, x, y):`

## inside the circle

Python tkinter example: inside the circle

```python
from tkinter import * # Import tkinter

width = 240
height = 120
        
class MainGUI:
    def __init__(self):
        window = Tk() # Create a window
        window.title("Inside the circle?") # Set a title
        
        self.canvas = Canvas(window, bg = "white", width = width, height = height)
        self.canvas.pack()
        self.canvas.create_oval(100 - 50, 60 - 50, 100 + 50, 60 + 50, tags = "circle")
        
        self.canvas.bind("<B1-Motion>", self.isInside)
        
        window.mainloop() # Create an event loop
        
    def isInside(self, event):
        self.canvas.delete("text")
        if isInsideCircle(100, 60, 50, event.x, event.y):
            self.canvas.create_text(event.x, event.y - 5, 
                               text = "Mouse pointer is in the circle", tags = "text")
        else:
            self.canvas.create_text(event.x, event.y - 5, 
                               text = "Mouse pointer is not in the circle", tags = "text")

def isInsideCircle(xCenter, yCenter, radius, x, y):
    return distance(xCenter, yCenter, x, y) <= radius
    
def distance(xCenter, yCenter, x, y):
    return ((xCenter - x) * (xCenter - x) + (yCenter - y) * (yCenter - y)) ** 0.5;

MainGUI()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
