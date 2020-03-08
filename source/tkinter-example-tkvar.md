---
title: tkinter example tkvar (snippet)
date: 2020-02-09
tags: ["python"]
---
Python tkinter (gui) example 'tkvar'

Functions in program: 
* `def varwrite(*args):`

Modules used in program: 
* `import Tkinter as Tk`

## tkvar

Python tkinter example: tkvar

```python
import Tkinter as Tk

root=Tk.Tk()
root.title("Tkvar")

frame1=Tk.Frame(root,bg="blue")
frame1.grid(row=0,column=0)#,sticky='n')

tkvar=Tk.StringVar()
tkvar.set("hello")
e1=Tk.Entry(frame1,textvariable=tkvar)
e1.grid(row=0,column=0,padx=20,pady=20)

def varwrite(*args):
    print("Write:",tkvar.get())

tkvar.trace("w", varwrite)

#print(e1.get())
root.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
