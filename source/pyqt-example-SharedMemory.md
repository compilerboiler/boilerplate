---
title: pyqt example SharedMemory (snippet)
date: 2020-02-10
tags: ["python"]
---
Python pyqt (gui) example 'SharedMemory'


## SharedMemory

Python pyqt example: SharedMemory

```python
#!/usr/bin/env python
# -*- coding: utf-8 -*-

'''
Created on 2017年3月30日
@author: Irony."[讽刺]
@site: https://pyqt5.com , https://github.com/892768447
@email: 892768447@qq.com
@file: TestQSharedMemory
@description: 
'''
from PyQt5.QtWidgets import QWidget


from Lib.Application import SharedApplication  # @UnresolvedImport

__version__ = "0.0.1"

class Widget(QWidget):
    
    def __init__(self,*args,**kwargs):
        super(Widget, self).__init__(*args,**kwargs)

if __name__ == "__main__":
    import sys,os
    print(os.getpid())
    app = SharedApplication(sys.argv)
    if app.isRunning():
        print("app have already running")
        sys.exit(0)
    w = Widget()
    w.show()
    sys.exit(app.exec_())

```

## Useful links

- Learn PyQt: https://pythonbasics.org/pyqt-hello-world/
- Install PyQt: https://pythonbasics.org/install-pyqt/
