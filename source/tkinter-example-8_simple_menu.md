---
title: tkinter example 8 simple menu (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example '8 simple menu'

Functions in program: 
* `def main():`

## 8 simple menu

Python tkinter example: 8 simple menu

```python
from Tkinter import Tk, Frame, Menu

class Window(Frame):

    def __init__(self, parent):
        Frame.__init__(self, parent)

        self.parent = parent

        self.startUI()

    def startUI(self):

        self.parent.title("Simple menu")

        menubar = Menu(self.parent)
        self.parent.config(menu=menubar)

        fileMenu = Menu(menubar)
        fileMenu.add_command(label="Exit", command=self.onExit)
        fileMenu.add_command(label="Bebs", command=self.bebs)

        helpMenu = Menu(menubar)
        helpMenu.add_command(label="help", command=self.help)


        menubar.add_cascade(label="File", menu=fileMenu)
        menubar.add_cascade(label="Help", menu=helpMenu)

    def onExit(self):
        self.quit()

    def bebs(self):
        print("bebs")

    def help(self):
        print("help")

def main():
    root = Tk()
    root.geometry("250x150+300+300")
    app = Window(root)
    root.mainloop()

if __name__ == '__main__':
    main()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
