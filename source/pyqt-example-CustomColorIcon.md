---
title: pyqt example CustomColorIcon (snippet)
date: 2020-02-10
tags: ["python"]
---
Python pyqt (gui) example 'CustomColorIcon'


Modules used in program: 
* `import sys`

## CustomColorIcon

Python pyqt example: CustomColorIcon

```python
#!/usr/bin/env python
# -*- coding: utf-8 -*-

'''
Created on 2018年1月17日
@author: Irony."[讽刺]
@site: https://pyqt5.com , https://github.com/892768447
@email: 892768447@qq.com
@file: CustomBtnIcon
@description: 
'''

__Author__ = "By: Irony.\"[讽刺]\nQQ: 892768447\nEmail: 892768447@qq.com"
__Copyright__ = "Copyright (c) 2018 Irony.\"[讽刺]"
__Version__ = "Version 1.0"

import sys

from PyQt5.QtWidgets import QApplication, QMessageBox


app = QApplication(sys.argv)
app.setStyleSheet('''QDialogButtonBox {
    dialogbuttonbox-buttons-have-icons: 1;
    dialog-ok-icon: url(Data/icons/Ok.png);
    dialog-open-icon: url(Data/icons/Open.png);
    dialog-save-icon: url(Data/icons/Save.png);
    dialog-cancel-icon: url(Data/icons/Cancel.png);
}

#qt_msgbox_label {
    color: red;
    background: green;
}

#qt_msgboxex_icon_label {
    background: red;
}

QMessageBox {
    background: black;
    messagebox-information-icon: url(Data/icons/Close.png);
}

QMessageBox QPushButton {
    padding: 2px;
    border-radius: 5px;
    background: white;
}

QMessageBox QPushButton:hover {
    background: darkCyan;
}

QMessageBox QPushButton[text="Reset"] {
    background: red;
}

QMessageBox QPushButton[text="Apply"] {
    background: cyan;
    qproperty-icon: url(Data/icons/Apply.png);
}
''')
QMessageBox.information(None, "information", "消息",
                     QMessageBox.Apply |
                     QMessageBox.Cancel |
                     QMessageBox.Close |
                     QMessageBox.Discard |
                     QMessageBox.Help |
                     QMessageBox.No |
                     QMessageBox.Ok |
                     QMessageBox.Open |
                     QMessageBox.Reset |
                     QMessageBox.Save |
                     QMessageBox.Yes)
sys.exit()


```

## Useful links

- Learn PyQt: https://pythonbasics.org/pyqt-hello-world/
- Install PyQt: https://pythonbasics.org/install-pyqt/
