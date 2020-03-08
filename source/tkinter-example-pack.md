---
title: tkinter example pack (snippet)
date: 2020-02-09
tags: ["python"]
---
Python tkinter (gui) example 'pack'


## pack

Python tkinter example: pack

```python
from Tkinter import *

root = Tk()
'''
w = Label(root, text="Red", bg="red", fg="white")
w.pack(fill=X)
w = Label(root, text="Green", bg="green", fg="black")
w.pack(fill=X,padx=10)
w = Label(root, text="Blue", bg="blue", fg="white")
w.pack(fill=X)

'''

root = Tk()

w = Label(root, text="Red", bg="red", fg="white")
w.pack(side=LEFT)
w = Label(root, text="Green", bg="green", fg="black")
w.pack(side=LEFT)
w = Label(root, text="Blue", bg="blue", fg="white")
w.pack(side=LEFT)

mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
