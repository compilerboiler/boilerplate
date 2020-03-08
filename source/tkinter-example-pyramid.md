---
title: tkinter example pyramid (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example 'pyramid'


## pyramid

Python tkinter example: pyramid

```python
from tkinter import * # Import tkinter

class MainGUI:
    def __init__(self):
        window = Tk() # Create a window
        window.title("Pyramid") # Set a title
        
        width = 150
        height = 150
        canvas = Canvas(window, bg = "white", width = width, height = height)
        canvas.pack()
        
        for i in range(1, 12): # Draw 8 horizontal lines
            s = ""
            for j in range(1, i + 1):
                s += str(j) + " "
            canvas.create_text(width / 2, i * height / 12, text = s, fill = "red")
            
        window.mainloop() # Create an event loop
        
MainGUI()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
