---
title: tkinter example dynamicContentInLabel (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example 'dynamicContentInLabel'

Functions in program: 
* `def counter_label(label):`

Modules used in program: 
* `import tkinter as tk`

## dynamicContentInLabel

Python tkinter example: dynamicContentInLabel

```python
import tkinter as tk

counter = 0


def counter_label(label):
    counter = 0

    def count():
        global counter
        counter += 1
        label.config(text=str(counter))
        # Calls count() after every 1000ms
        label.after(1000, count)

    count()


root = tk.Tk()
root.title("Counting Seconds")
label = tk.Label(root, fg="dark green")
label.pack()
counter_label(label)
button = tk.Button(root, text='Stop', width=25, command=root.destroy)
button.pack()
root.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
