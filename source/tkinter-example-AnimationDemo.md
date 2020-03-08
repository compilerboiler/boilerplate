---
title: tkinter example AnimationDemo (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example 'AnimationDemo'


## AnimationDemo

Python tkinter example: AnimationDemo

```python
from tkinter import * # Import tkinter

class AnimationDemo:
    def __init__(self):
        window = Tk() # Create a window
        window.title("Animation Demo") # Set a title
        
        width = 250 # Width of the canvas
        canvas = Canvas(window, bg = "white", 
            width = 250, height = 50)
        canvas.pack()
        
        x = 0 # Starting x position
        canvas.create_text(x, 30, 
            text = "Message moving?", tags = "text")
        
        dx = 3
        while True:
            canvas.move("text", dx, 0) # Move text dx unit
            canvas.after(100) # Sleep for 100 milliseconds
            canvas.update() # Update canvas
            if x < width:
                x += dx  # Get the current position for string
            else:
                x = 0 # Reset string position to the beginning
                canvas.delete("text") 
                # Redraw text at the beginning
                canvas.create_text(x, 30, text = "Message moving?", 
                    tags = "text")
                
        window.mainloop() # Create an event loop

AnimationDemo() # Create GUI

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
