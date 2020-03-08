---
title: tkinter example DialogDemo (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example 'DialogDemo'


Modules used in program: 
* `import tkinter.colorchooser`
* `import tkinter.simpledialog`
* `import tkinter.messagebox`

## DialogDemo

Python tkinter example: DialogDemo

```python
import tkinter.messagebox
import tkinter.simpledialog
import tkinter.colorchooser

tkinter.messagebox.showinfo("showinfo", "This is an info msg")

tkinter.messagebox.showwarning("showwarning", "This is a warning")

tkinter.messagebox.showerror("showerror", "This is an error")

isYes = tkinter.messagebox.askyesno("ashyesno", "Continue?")
print(isYes)

isOK = tkinter.messagebox.askokcancel("ashokcancle", "OK?")
print(isOK)

isYesNoCancel = tkinter.messagebox.askyesnocancel(
    "askyesnocancel", "Yes, No, Cancel?") 
print(isYesNoCancel)

name = tkinter.simpledialog.askstring(
    "askstring", "Enter your name")
print(name)

age = tkinter.simpledialog.askinteger(
    "askinteger", "Enter your age")
print(age)

weight = tkinter.simpledialog.askfloat(
    "askfloat", "Enter your weight")
print(weight)


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
