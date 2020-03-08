---
title: tkinter example 5 buttons example (snippet)
date: 2020-02-09
tags: ["python"]
---
Python tkinter (gui) example '5 buttons example'

Functions in program: 
* `def main():`

## 5 buttons example

Python tkinter example: 5 buttons example

```python
from Tkinter import Tk, RIGHT, BOTH, RAISED
from ttk import Frame, Button, Style

class Example(Frame):
    def __init__(self, parent):
        Frame.__init__(self, parent)

        self.parent = parent

        self.initUI()

    def initUI(self):

        self.parent.title("Buttons")
        self.style = Style()
        self.style.theme_use("default")

        frame = Frame(self, relief=RAISED, borderwidth=1)
        frame.pack(fill=BOTH, expand=1)

        frame2 = Frame(self, relief=RAISED, borderwidth=2)
        frame2.pack(fill=BOTH, expand=1)

        self.pack(fill=BOTH, expand=1)

        closeButton = Button(self, text="Close")
        closeButton.pack(side=RIGHT, padx=5, pady=5)
        okButton = Button(self, text="OK")
        okButton.pack(side=RIGHT)

def main():

    root = Tk()
    root.geometry("300x200+300+300")
    app = Example(root)
    root.mainloop()

if __name__ == '__main__':
    main()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
