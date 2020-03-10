---
title: pyqt example FlipWidgetAnimation (snippet)
date: 2020-02-10
tags: ["python"]
---
Python pyqt (gui) example 'FlipWidgetAnimation'


## FlipWidgetAnimation

Python pyqt example: FlipWidgetAnimation

```python
#!/usr/bin/env python
# -*- coding: utf-8 -*-

"""
Created on 2019年5月15日
@author: Irony
@site: https://pyqt5.com https://github.com/892768447
@email: 892768447@qq.com
@file: 翻转动画
@description: 
"""
from PyQt5.QtCore import Qt, pyqtSignal, QTimer
from PyQt5.QtGui import QPixmap
from PyQt5.QtWidgets import QStackedWidget, QLabel

from Lib.FlipWidget import FlipWidget


__Author__ = 'Irony'
__Copyright__ = 'Copyright (c) 2019 Irony'
__Version__ = 1.0


class LoginWidget(QLabel):
    # 只是显示登录界面截图

    windowClosed = pyqtSignal()
    windowChanged = pyqtSignal()

    def __init__(self, *args, **kwargs):
        super(LoginWidget, self).__init__(*args, **kwargs)
        self.setPixmap(QPixmap('Data/1.png'))

    def mousePressEvent(self, event):
        super(LoginWidget, self).mousePressEvent(event)
        pos = event.pos()
        if pos.y() <= 40:
            if pos.x() > self.width() - 30:
                # 点击关闭按钮的地方
                self.windowClosed.emit()
            elif self.width() - 90 <= pos.x() <= self.width() - 60:
                # 点击切换按钮
                self.windowChanged.emit()


class SettingWidget(QLabel):
    # 只是显示设置界面截图

    windowClosed = pyqtSignal()
    windowChanged = pyqtSignal()

    def __init__(self, *args, **kwargs):
        super(SettingWidget, self).__init__(*args, **kwargs)
        self.setPixmap(QPixmap('Data/2.png'))

    def mousePressEvent(self, event):
        super(SettingWidget, self).mousePressEvent(event)
        pos = event.pos()
        if pos.y() >= self.height() - 30:
            if self.width() - 95 <= pos.x() <= self.width() - 10:
                # 点击切换按钮
                self.windowChanged.emit()
        elif pos.y() <= 40:
            if pos.x() > self.width() - 30:
                # 点击关闭按钮的地方
                self.windowClosed.emit()


class Window(QStackedWidget):
    # 主窗口

    def __init__(self, *args, **kwargs):
        super(Window, self).__init__(*args, **kwargs)
        self.resize(428, 329)
        self.setWindowFlags(self.windowFlags() | Qt.FramelessWindowHint)

        # 这个是动画窗口，先创建不显示
        self.flipWidget = FlipWidget()
        self.flipWidget.finished.connect(self.showWidget)

        # 登录窗口
        self.loginWidget = LoginWidget(self)
        self.loginWidget.windowClosed.connect(self.close)
        self.loginWidget.windowChanged.connect(self.jumpSettingWidget)
        self.addWidget(self.loginWidget)

        # 设置窗口
        self.settingWidget = SettingWidget(self)
        self.settingWidget.windowClosed.connect(self.close)
        self.settingWidget.windowChanged.connect(self.jumpLoginWidget)
        self.addWidget(self.settingWidget)

    def showWidget(self):
        # 显示主窗口隐藏动画窗口
        self.setWindowOpacity(1)
        QTimer.singleShot(100, self.flipWidget.hide)

    def jumpLoginWidget(self):
        # 翻转到登录界面
        self.setWindowOpacity(0)                 # 类似隐藏，但是保留了任务栏
        self.setCurrentWidget(self.loginWidget)  # 很重要，一定要先切换过去，不然会导致第一次截图有误
        image1 = self.loginWidget.grab()       # 截图1
        image2 = self.settingWidget.grab()     # 截图2
        padding = 100                          # 扩大边距 @UnusedVariable
        self.flipWidget.setGeometry(self.geometry())
        # .adjusted(-padding, -padding, padding, padding))
        self.flipWidget.updateImages(FlipWidget.Right, image2, image1)

    def jumpSettingWidget(self):
        # 翻转到设置界面
        self.setWindowOpacity(0)                  # 类似隐藏，但是保留了任务栏
        self.setCurrentWidget(self.settingWidget)  # 很重要，一定要先切换过去，不然会导致第一次截图有误
        image1 = self.loginWidget.grab()       # 截图1
        image2 = self.settingWidget.grab()     # 截图2
        padding = 100                          # 扩大边距 @UnusedVariable
        self.flipWidget.setGeometry(self.geometry())
        # .adjusted(-padding, -padding, padding, padding))
        self.flipWidget.updateImages(FlipWidget.Left, image1, image2)


if __name__ == '__main__':
    import sys
    from PyQt5.QtWidgets import QApplication
    app = QApplication(sys.argv)
    w = Window()
    w.show()
    sys.exit(app.exec_())


```

## Useful links

- Learn PyQt: https://pythonbasics.org/pyqt-hello-world/
- Install PyQt: https://pythonbasics.org/install-pyqt/