---
title: tkinter example 11 file dialog (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example '11 file dialog'

Functions in program: 
* `def main():`

Modules used in program: 
* `import tkFileDialog`

## 11 file dialog

Python tkinter example: 11 file dialog

```python
from Tkinter import Frame, Tk, BOTH, Text, Menu, END
import tkFileDialog

class Window(Frame):

    def __init__(self, parent):
        Frame.__init__(self, parent)

        self.parent = parent

        self.startUI()


    def startUI(self):

        self.parent.title("File dialog")
        self.pack(fill=BOTH, expand=1)

        menubar = Menu(self.parent)
        self.parent.config(menu=menubar)

        fileMenu = Menu(menubar)
        fileMenu.add_command(label="Open", command=self.onOpen)
        fileMenu.add_command(label="Exit", command=self.quit)

        
        menubar.add_cascade(label="File", menu=fileMenu)

        self.txt = Text(self)
        self.txt.pack(fill=BOTH, expand=1)

    def onOpen(self):

        ftypes = [('Python files', '*.py'), ('All files', '*.*')]
        dlg = tkFileDialog.Open(self, filetypes = ftypes)
        fl = dlg.show()

        if fl != '':
            text = self.readFile(fl)
            self.txt.insert(END, text)

    def readFile(self, filename):

        f = open(filename, "r")
        text = f.read()
        f.close()
        return text

def main():
    root = Tk()
    ex = Window(root)
    root.geometry("300x250+300+300")
    root.mainloop()

if __name__ == '__main__':
    main()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
