---
title: tkinter example button (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example 'button'


Modules used in program: 
* `import Tkinter as Tk`

## button

Python tkinter example: button

```python
import Tkinter as Tk

root=Tk.Tk()
root.title("Hello World")

frame1=Tk.Frame(root,bg="blue",height=200,width=400)
frame1.grid(row=1,column=1)#,sticky='n')

Tk.Button(frame1,text="Click to quit",command=quit).grid(row=0,column=0,padx=20,pady=20)

root.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
