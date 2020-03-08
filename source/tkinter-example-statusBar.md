---
title: tkinter example statusBar (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example 'statusBar'

Functions in program: 
* `def ButtonQuitHandler(statusBar, root):`
* `def ButtonTestHandler(statusBar):`

Modules used in program: 
* `import tkinter.messagebox`

## statusBar

Python tkinter example: statusBar

```python
from tkinter import *
import tkinter.messagebox

############################################################################
# Status bar class
############################################################################
class StatusBar:
    #######################################################################
    # Constructor
    # @param root   : Window in which this status bar should lie
    # @param width  : Width of the status bar
    #######################################################################
    def __init__(self, root, width):
        self.frame = Frame(root, padx=2, pady=2)
        self.frame.pack(side=BOTTOM)

        self.lblTitle = Label(self.frame, text="Status: ")
        self.lblTitle.pack(side=LEFT)

        self.lblStatusBar = Label(self.frame, text="Welcome", width=width, bd=1, relief=SUNKEN)
        self.lblStatusBar.pack(side=RIGHT)

    def Set(self, value):
        self.lblStatusBar.config(text=value)

############################################################################
# Global functions
############################################################################
def ButtonTestHandler(statusBar):
    statusBar.Set("Clicked Test button")

def ButtonQuitHandler(statusBar, root):
    statusBar.Set("Clicked on Quit")
    response = str(tkinter.messagebox.askquestion("Quit", "Are you sure you want to quit?"))
    statusBar.Set("{} selected".format(response))

    if (response == "yes"):
        statusBar.Set("Quitting")
        root.quit()
    else:
        statusBar.Set("Ignoring")


############################################################################
# Main
############################################################################
root = Tk()
root.title("Status bar test window")


sb = StatusBar(root, 20)

btnTest = Button(root, text="Test", command=lambda:ButtonTestHandler(sb))
btnTest.pack(side=LEFT)

btnQuit = Button(root, text="Quit", command=lambda:ButtonQuitHandler(sb, root))
btnQuit.pack(side=RIGHT)

root.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
