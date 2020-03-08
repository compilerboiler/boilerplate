---
title: tkinter example grid (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example 'grid'


Modules used in program: 
* `import Tkinter`

## grid

Python tkinter example: grid

```python
import Tkinter
root = Tkinter.Tk(  )
for r in range(3):
   for c in range(4):
      Tkinter.Label(root, text='Row%s/Column%s'%(r,c),fg="red",
         padx=5,pady=5 ).grid(row=r,column=c)
root.mainloop( )


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
