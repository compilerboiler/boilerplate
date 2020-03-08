---
title: tkinter example radiobutton (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example 'radiobutton'


Modules used in program: 
* `import Tkinter as Tk`

## radiobutton

Python tkinter example: radiobutton

```python
import Tkinter as Tk

root = Tk.Tk()

v = Tk.IntVar()

Tk.Label(root,text="""Choose a 
programming language:""",justify = Tk.LEFT,
        padx = 20).pack()
Tk.Radiobutton(root,text="Python",padx = 20,variable=v,value=1).pack(anchor=Tk.W)
Tk.Radiobutton(root,text="Perl",padx = 20,variable=v,value=2).pack(anchor=Tk.W)

root.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
