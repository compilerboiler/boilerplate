---
title: pyqt example HighlightText (snippet)
date: 2020-02-10
tags: ["python"]
---
Python pyqt (gui) example 'HighlightText'


Modules used in program: 
* `import sys`

## HighlightText

Python pyqt example: HighlightText

```python
import sys
from PyQt5.QtGui import QTextCharFormat, QTextDocument, QTextCursor
from PyQt5.QtWidgets import (QApplication, QMainWindow, QTextEdit,
                             QToolBar, QLineEdit, QPushButton, QColorDialog, QHBoxLayout, QWidget)


class TextEdit(QMainWindow):
    def __init__(self, parent=None):
        super(TextEdit, self).__init__(parent)
        self.textEdit = QTextEdit(self)
        self.setCentralWidget(self.textEdit)

        widget = QWidget(self)
        vb = QHBoxLayout(widget)
        vb.setContentsMargins(0, 0, 0, 0)
        self.findText = QLineEdit(self)
        self.findText.setText('self')
        findBtn = QPushButton('高亮', self)
        findBtn.clicked.connect(self.highlight)
        vb.addWidget(self.findText)
        vb.addWidget(findBtn)

        tb = QToolBar(self)
        tb.addWidget(widget)

    def setText(self, text):
        self.textEdit.setPlainText(text)

    def mergeFormatOnWordOrSelection(self, format):
        cursor = self.textEdit.textCursor()
        if not cursor.hasSelection():
            cursor.select(QTextCursor.WordUnderCursor)
        cursor.mergeCharFormat(format)
        self.textEdit.mergeCurrentCharFormat(format)

    def highlight(self):
        text = self.findText.text()  # 输入框中的文字
        if not text:
            return
        col = QColorDialog.getColor(self.textEdit.textColor(), self)
        if not col.isValid():
            return
        fmt = QTextCharFormat()
        fmt.setForeground(col)
        # 先把光标移动到开头
        self.textEdit.moveCursor(QTextCursor.Start)
        while self.textEdit.find(text, QTextDocument.FindWholeWords):  # 查找所有文字
            self.mergeFormatOnWordOrSelection(fmt)


if __name__ == '__main__':
    app = QApplication(sys.argv)

    textEdit = TextEdit()
    textEdit.resize(800, 600)
    textEdit.show()
    textEdit.setText(open(sys.argv[0], 'rb').read().decode())

    sys.exit(app.exec_())


```

## Useful links

- Learn PyQt: https://pythonbasics.org/pyqt-hello-world/
- Install PyQt: https://pythonbasics.org/install-pyqt/
