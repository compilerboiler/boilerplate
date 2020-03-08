---
title: tkinter example 27-gui-frames (snippet)
date: 2019-02-08
tags: ["python"]
---
Python tkinter (gui) example '27-gui-frames'


## 27-gui-frames

Python tkinter example: 27-gui-frames

```python
from tkinter import *

# main window and 2 frames
my_window = Tk()
frame_name = Frame(my_window)
frame_address = Frame(my_window)

# build the GUI
# Name Frame
label_first = Label(frame_name, text='First Name')
label_middle = Label(frame_name, text='Middle Name')
label_surname = Label(frame_name, text='Last Name')

entry_first = Entry(frame_name)
entry_middle = Entry(frame_name)
entry_surname = Entry(frame_name)

button_submit_name = Button(frame_name, text='Submit')

label_first.grid(row=0, column=0) # respecto a su frame_name
label_middle.grid(row=1, column=0)
label_surname.grid(row=2, column=0)

entry_first.grid(row=0, column=1)
entry_middle.grid(row=1, column=1)
entry_surname.grid(row=2, column=1)

button_submit_name.grid(row=3, columnspan=2)

# address frame
label_first_line = Label(frame_address, text='First Line')
label_town = Label(frame_address, text='Town')
label_country = Label(frame_address, text='Country')

entry_first_line = Entry(frame_address)
entry_town = Entry(frame_address)
entry_country = Entry(frame_address)

button_submit_address = Button(frame_address, text='Submit')

label_first_line.grid(row=0, column=0) # respecto a su frame_name
label_town.grid(row=1, column=0)
label_country.grid(row=2, column=0)

entry_first_line.grid(row=0, column=1)
entry_town.grid(row=1, column=1)
entry_country.grid(row=2, column=1)

button_submit_address.grid(row=3, columnspan=2)

# adding frames to main window
frame_name.grid(row=0, column=0) # respecto a my_window
frame_address.grid(row=1, column=0)

# Focus
entry_first.focus()

my_window.mainloop()


```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter
