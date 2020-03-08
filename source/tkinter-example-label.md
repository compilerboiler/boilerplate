---
title: tkinter example label (snippet)
date: 2020-02-09
tags: ["python"]
---
Python tkinter (gui) example 'label'


Modules used in program: 
* `import Tkinter as Tk`

## label

Python tkinter example: label

```python
import Tkinter as Tk

root=Tk.Tk()
root.title("Hello World")

frame1=Tk.Frame(root,bg="blue",height=200,width=400)
frame1.grid(row=1,column=1)#,sticky='n')

Tk.Label(frame1,text="Demonstrating Label widget",bg="white").grid(row=0,column=0,padx=20,pady=20)

root.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
