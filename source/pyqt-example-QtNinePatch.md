---
title: pyqt example QtNinePatch (snippet)
date: 2020-02-10
tags: ["python"]
---
Python pyqt (gui) example 'QtNinePatch'


Modules used in program: 
* `import sys`

## QtNinePatch

Python pyqt example: QtNinePatch

```python
#!/usr/bin/env python
# -*- coding: utf-8 -*-

"""
Created on 2018年10月25日
@author: Irony
@site: https://pyqt5.com , https://github.com/892768447
@email: 892768447@qq.com
@file: testQtNinePatch
@description: 
"""


__Author__ = """By: Irony
QQ: 892768447
Email: 892768447@qq.com"""
__Copyright__ = "Copyright (c) 2018 Irony"
__Version__ = "Version 1.0"

import sys

from ctypes import CDLL
from PyQt5.QtGui import QImage
from PyQt5.QtWidgets import QApplication, QLabel

CDLL('Lib/QtNinePatch/sip/QtNinePatch.dll')

from Lib.QtNinePatch.sip.QtNinePatch import QtNinePatch


class Label(QLabel):

    def __init__(self, *args, **kwargs):
        super(Label, self).__init__(*args, **kwargs)
        #.9 格式的图片
        self.image = QImage('Data/skin_aio_friend_bubble_pressed.9.png')

    def showEvent(self, event):
        super(Label, self).showEvent(event)
        pixmap = QtNinePatch.createPixmapFromNinePatchImage(
            self.image, self.width(), self.height())
        self.setPixmap(pixmap)

    def resizeEvent(self, event):
        super(Label, self).resizeEvent(event)
        pixmap = QtNinePatch.createPixmapFromNinePatchImage(
            self.image, self.width(), self.height())
        self.setPixmap(pixmap)


app = QApplication(sys.argv)
w = Label()
w.resize(400, 200)
w.show()

sys.exit(app.exec_())


```

## Useful links

- Learn PyQt: https://pythonbasics.org/pyqt-hello-world/
- Install PyQt: https://pythonbasics.org/install-pyqt/
