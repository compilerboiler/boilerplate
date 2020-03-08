---
title: tkinter example TK Example1 (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example 'TK Example1'

Functions in program: 
* `def main():`

## TK Example1

Python tkinter example: TK Example1

```python
from tkinter import *
"""Our very basic Tkinter Application
This just creates a window with no widgets."""

class App(Frame):
    """Our Application. We inherit all the properties
    and methods of a Tkinter Frame"""
    def __init__(self,master=None):
        Frame.__init__(self,master)

def main():
    root = Tk()
    app = App(master=root)

"""This is the code that is executed by python when we run this .py file"""
if __name__ == '__main__':
    main()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
