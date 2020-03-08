---
title: tkinter example 1 tkinter example (snippet)
date: 2020-02-09
tags: ["python"]
---
Python tkinter (gui) example '1 tkinter example'

Functions in program: 
* `def main():`

## 1 tkinter example

Python tkinter example: 1 tkinter example

```python
from Tkinter import Tk, Frame, BOTH

class Example(Frame):

    def __init__(self, parent):
        Frame.__init__(self, parent, background="white")

        self.parent = parent

        self.initUI()

    def initUI(self):
        self.parent.title("Simple")
        self.pack(fill=BOTH, expand=1)

def main():
    root = Tk()
    root.geometry("250x150+300+300")
    app = Example(root)
    root.mainloop()

if __name__ == '__main__':
    main()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
