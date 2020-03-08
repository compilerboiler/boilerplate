---
title: tkinter example TK Example2 (snippet)
date: 2020-02-09
tags: ["python"]
---
Python tkinter (gui) example 'TK Example2'

Functions in program: 
* `def main():`

## TK Example2

Python tkinter example: TK Example2

```python
from tkinter import *
"""A simple hello world example
We create a label inside our application with the text Hello World and
configure the foreground colour to be red."""

class App(Frame):
    """Our Application. We inherit all the properties
    and methods of a Tkinter Frame"""
    def __init__(self,master=None):
        Frame.__init__(self,master)
        self.lblHello = Label(self,text="Hello World")
        self.lblHello['fg'] = "red"
        self.lblHello.grid()
        self.btnStart = Button(self,text="Click Me")
        self.btnStart.grid()

def main():
    root = Tk()
    app = App(master=root)
    app.grid()

"""This is the code that is executed by python when we run this .py file"""
if __name__ == '__main__':
    main()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
