---
title: tkinter example fileBrowse (snippet)
date: 2020-02-02
tags: ["python"]
---
Python tkinter (gui) example 'fileBrowse'

Functions in program: 
* `def BrowseFile():`
* `def BrowseDir():`

## fileBrowse

Python tkinter example: fileBrowse

```python
from tkinter import filedialog
from tkinter import *

DEFAULT_FILE_PATH = r"C:\Users\m0pxnn\Documents\Python"
filename = "<NOTHING SELECTED>"
folderName = "<Folder not selected>"

def BrowseDir():
    folderName = filedialog.askdirectory(initialdir=DEFAULT_FILE_PATH, title="Select folder")
    print("Folder selected: ", folderName)
    lblFilename['text'] = "Folder selected: " + folderName

def BrowseFile():
    filename = filedialog.askopenfilename(initialdir=DEFAULT_FILE_PATH, title="Select file",
                                               filetypes=(("jpeg files", "*.jpg"), ("all files", "*.*")))
    print("File selected: ", filename)
    lblFilename['text'] = "File selected: " + filename

#############################################
root = Tk()

btnBrowseFile = Button(root, text="Browse File", command=BrowseFile)
btnBrowseFile.pack()

btnBrowseDir = Button(root, text="Browse Folder", command=BrowseDir)
btnBrowseDir.pack()

lblFilename = Label(root, text=filename, width=100, padx=2, pady=2, bd=2, relief=RIDGE  )
lblFilename.pack()

'''
# Relief styles
B1 = Button(root, text ="FLAT", relief=FLAT )
B2 = Button(root, text ="RAISED", relief=RAISED )
B3 = Button(root, text ="SUNKEN", relief=SUNKEN )
B4 = Button(root, text ="GROOVE", relief=GROOVE )
B5 = Button(root, text ="RIDGE", relief=RIDGE )

B1.pack()
B2.pack()
B3.pack()
B4.pack()
B5.pack()
'''


root.mainloop()

```

## Useful links

- Learn Tkinter: https://pythonbasics.org/tkinter/
- Wikipedia tkinter: https://en.wikipedia.org/wiki/Tkinter