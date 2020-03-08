---
title: tkinter example arrow keys (snippet)
date: 2020-02-09
tags: ["python"]
---
Python tkinter (gui) example 'arrow keys'


## arrow keys

Python tkinter example: arrow keys

```python
from tkinter import * # Import tkinter

width = 220
height = 100

class MainGUI:
    def __init__(self):
        window = Tk() # Create a window
        window.title("Arrow Keys") # Set a title

        self.canvas = Canvas(window, bg = "white", width = width, height = height)
        self.canvas.pack()
        
        # Bind canvas with key events
        self.canvas.bind("<Up>", self.up)
        self.canvas.bind("<Down>", self.down)
        self.canvas.bind("<Left>", self.left)
        self.canvas.bind("<Right>", self.right)
        self.canvas.focus_set()
        
        self.x = width / 2
        self.y = height / 2

        window.mainloop() # Create an event loop

    def up(self, event):
        self.canvas.create_line(self.x, self.y, self.x, self.y - 5, tags = "line")
        self.y -= 5
        
    def down(self, event):
        self.canvas.create_line(self.x, self.y, self.x, self.y + 5, tags = "line")
        self.y += 5
        
    def left(self, event):
        self.canvas.create_line(self.x, self.y, self.x - 5, self.y, tags = "line")
        self.x -= 5
    
    def right(self, event):
        self.canvas.create_line(self.x, self.y, self.x + 5, self.y, tags = "line")
        self.x += 5

MainGUI()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
