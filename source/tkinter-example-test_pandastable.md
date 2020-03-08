---
title: tkinter example test pandastable (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example 'test pandastable'


## test pandastable

Python tkinter example: test pandastable

```python
from tkinter import *
from pandastable import Table, TableModel

class TestApp(Frame):
        """Basic test frame for the table"""
        def __init__(self, parent=None):
            self.parent = parent
            Frame.__init__(self)
            self.main = self.master
            self.main.geometry('600x400+200+100')
            self.main.title('Table app')
            f = Frame(self.main)
            f.pack(fill=BOTH,expand=1)
            df = TableModel.getSampleData()
            self.table = pt = Table(f, dataframe=df,
                                    showtoolbar=True, showstatusbar=True)
            pt.show()
            return

app = TestApp()
#launch the app
try:
    app.mainloop()
except UnicodeDecodeError:
    pass


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
