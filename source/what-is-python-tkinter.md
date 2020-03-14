---
date: 2020-02-16
title: what is python tkinter
---
To make a graphical user interface, you can use the tkinter module. <a href="https://docs.python.org/3/library/tkinter.html">Tkinter</a> is a module for GUIs (based on the Tk GUI toolkit).  

This is the standard graphical user interface for Python. Tkinter is included with Linux, Microsoft Windows and Mac OS X.

Of course there are other GUI modules like <a href="https://pythonspot.com/pyqt5/">PyQt</a>, <a href="https://pygobject.readthedocs.io/en/latest/">PyGTK</a>, <a href="https://pypi.org/project/simplegui/">simpleGUI</a> and others. One of the advantages of tkinter is that it's included by default and you can learn it quickly.

![tkinter app](https://dev-to-uploads.s3.amazonaws.com/i/zgg6t3imnvrh2au77kkx.png)

## Example

With tkinter you can quickly build graphical interfaces. The example below shows you the hello world app.

```python
from tkinter import *

root = Tk()

w = Label(root, text="Hello, world!")
w.pack()

root.mainloop()
```

![tkinter hello world](https://dev-to-uploads.s3.amazonaws.com/i/alhmvnlpy4qjqyxrysas.png)

It loads the module like this:

```python
from tkinter import *
```

If you get an import error, make sure you are using Python version 3 or newer.

    python --version

Then tk (root window) is initialized with:


```python
root = Tk()
```

A label with the text "Hello world" is created and added to the root window

```python
w = Label(root, text="Hello, world!")
w.pack()
```

You can add many widgets to your window like <a href="https://pythonbasics.org/tkinter-button/">buttons</a>, <a href="https://pythonbasics.org/tkinter-menu/">file menu</a>, <a href="https://pythonbasics.org/tkinter-image/">images</a> an <a href="https://pythonbasics.org/tkinter-entry/">input box</a> and others.

**Related links:**
* <a href="https://docs.python.org/3/library/tkinter.html">Tkinter documentation</a>
* <a href="https://gumroad.com/l/ErLc">Tkinter video course</a>
