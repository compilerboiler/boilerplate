---
title: tkinter example message (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example 'message'

Functions in program: 
* `def hit_me():`

Modules used in program: 
* `import tkinter as tk`

## message

Python tkinter example: message

```python
# -*- coding: utf-8 -*-
from __future__ import unicode_literals
import tkinter as tk

window = tk.Tk()
window.geometry('200x200')

def hit_me():
	# 声明一个弹窗 messagebox. 其他的类型还有:
	#	showwarning
	#	showerror
	#	askquestion
	#	askyesno
	#	asktrycancel
	tk.messagebox.showinfo(title='Hit me', message='hahahah')

tk.Button(
		window,
		text='Click me',
		command=hit_me
	).pack()

window.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
