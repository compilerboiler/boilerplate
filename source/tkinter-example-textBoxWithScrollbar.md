---
title: tkinter example textBoxWithScrollbar (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example 'textBoxWithScrollbar'


Modules used in program: 
* `import tkinter as tk`

## textBoxWithScrollbar

Python tkinter example: textBoxWithScrollbar

```python
import tkinter as tk

root = tk.Tk()

S = tk.Scrollbar(root)
T = tk.Text(root, height=4, width=50)

S.pack(side=tk.RIGHT, fill=tk.Y)
T.pack(side=tk.LEFT, fill=tk.Y)

S.config(command=T.yview)
T.config(yscrollcommand=S.set)

quote = """HAMLET: To be, or not to be--that is the question:
Whether 'tis nobler in the mind to suffer
The slings and arrows of outrageous fortune
Or to take arms against a sea of troubles
And by opposing end them. To die, to sleep--
No more--and by a sleep to say we end
The heartache, and the thousand natural shocks
That flesh is heir to. 'Tis a consummation
Devoutly to be wished."""

T.insert(tk.END, quote)
tk.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
