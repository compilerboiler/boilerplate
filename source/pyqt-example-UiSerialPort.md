---
title: pyqt example UiSerialPort (snippet)
date: 2020-02-10
tags: ["python"]
---
Python pyqt (gui) example 'UiSerialPort'


## UiSerialPort

Python pyqt example: UiSerialPort

```python
# -*- coding: utf-8 -*-

# Form implementation generated from reading ui file 'UiSerialPort.ui'
#
# Created by: PyQt5 UI code generator 5.10.1
#
# WARNING! All changes made in this file will be lost!

from PyQt5 import QtCore, QtGui, QtWidgets

class Ui_FormSerialPort(object):
    def setupUi(self, FormSerialPort):
        FormSerialPort.setObjectName("FormSerialPort")
        FormSerialPort.resize(721, 597)
        FormSerialPort.setStyleSheet("#labelStatus {\n"
"    border-radius: 13px;\n"
"    background-color: gray;\n"
"}\n"
"#labelStatus[isOn=\"true\"] {\n"
"    background-color: green;\n"
"}")
        self.gridLayout = QtWidgets.QGridLayout(FormSerialPort)
        self.gridLayout.setObjectName("gridLayout")
        self.groupBox = QtWidgets.QGroupBox(FormSerialPort)
        self.groupBox.setTitle("")
        self.groupBox.setObjectName("groupBox")
        self.formLayout = QtWidgets.QFormLayout(self.groupBox)
        self.formLayout.setLabelAlignment(QtCore.Qt.AlignCenter)
        self.formLayout.setObjectName("formLayout")
        self.label = QtWidgets.QLabel(self.groupBox)
        self.label.setObjectName("label")
        self.formLayout.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label)
        self.comboBoxPort = QtWidgets.QComboBox(self.groupBox)
        self.comboBoxPort.setObjectName("comboBoxPort")
        self.formLayout.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.comboBoxPort)
        self.label_2 = QtWidgets.QLabel(self.groupBox)
        self.label_2.setObjectName("label_2")
        self.formLayout.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_2)
        self.comboBoxBaud = QtWidgets.QComboBox(self.groupBox)
        self.comboBoxBaud.setObjectName("comboBoxBaud")
        self.comboBoxBaud.addItem("")
        self.comboBoxBaud.addItem("")
        self.comboBoxBaud.addItem("")
        self.comboBoxBaud.addItem("")
        self.comboBoxBaud.addItem("")
        self.comboBoxBaud.addItem("")
        self.comboBoxBaud.addItem("")
        self.comboBoxBaud.addItem("")
        self.formLayout.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.comboBoxBaud)
        self.label_3 = QtWidgets.QLabel(self.groupBox)
        self.label_3.setObjectName("label_3")
        self.formLayout.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_3)
        self.comboBoxParity = QtWidgets.QComboBox(self.groupBox)
        self.comboBoxParity.setObjectName("comboBoxParity")
        self.comboBoxParity.addItem("")
        self.comboBoxParity.addItem("")
        self.comboBoxParity.addItem("")
        self.comboBoxParity.addItem("")
        self.comboBoxParity.addItem("")
        self.comboBoxParity.addItem("")
        self.formLayout.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.comboBoxParity)
        self.label_4 = QtWidgets.QLabel(self.groupBox)
        self.label_4.setObjectName("label_4")
        self.formLayout.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_4)
        self.comboBoxData = QtWidgets.QComboBox(self.groupBox)
        self.comboBoxData.setObjectName("comboBoxData")
        self.comboBoxData.addItem("")
        self.comboBoxData.addItem("")
        self.comboBoxData.addItem("")
        self.comboBoxData.addItem("")
        self.formLayout.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.comboBoxData)
        self.label_5 = QtWidgets.QLabel(self.groupBox)
        self.label_5.setObjectName("label_5")
        self.formLayout.setWidget(4, QtWidgets.QFormLayout.LabelRole, self.label_5)
        self.comboBoxStop = QtWidgets.QComboBox(self.groupBox)
        self.comboBoxStop.setObjectName("comboBoxStop")
        self.comboBoxStop.addItem("")
        self.comboBoxStop.addItem("")
        self.comboBoxStop.addItem("")
        self.comboBoxStop.addItem("")
        self.formLayout.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.comboBoxStop)
        self.buttonConnect = QtWidgets.QPushButton(self.groupBox)
        self.buttonConnect.setObjectName("buttonConnect")
        self.formLayout.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.buttonConnect)
        self.labelStatus = QtWidgets.QLabel(self.groupBox)
        self.labelStatus.setProperty("isOn", False)
        self.labelStatus.setObjectName("labelStatus")
        self.formLayout.setWidget(5, QtWidgets.QFormLayout.LabelRole, self.labelStatus)
        spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
        self.formLayout.setItem(6, QtWidgets.QFormLayout.FieldRole, spacerItem)
        self.gridLayout.addWidget(self.groupBox, 0, 0, 1, 1)
        self.textBrowser = QtWidgets.QTextBrowser(FormSerialPort)
        self.textBrowser.setObjectName("textBrowser")
        self.gridLayout.addWidget(self.textBrowser, 0, 1, 2, 1)
        self.widget = QtWidgets.QWidget(FormSerialPort)
        self.widget.setObjectName("widget")
        self.verticalLayout = QtWidgets.QVBoxLayout(self.widget)
        self.verticalLayout.setObjectName("verticalLayout")
        self.pushButton_2 = QtWidgets.QPushButton(self.widget)
        self.pushButton_2.setObjectName("pushButton_2")
        self.verticalLayout.addWidget(self.pushButton_2)
        self.checkBoxHexView = QtWidgets.QCheckBox(self.widget)
        self.checkBoxHexView.setObjectName("checkBoxHexView")
        self.verticalLayout.addWidget(self.checkBoxHexView)
        self.gridLayout.addWidget(self.widget, 1, 0, 1, 1)
        self.widget_2 = QtWidgets.QWidget(FormSerialPort)
        self.widget_2.setObjectName("widget_2")
        self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.widget_2)
        self.verticalLayout_2.setObjectName("verticalLayout_2")
        self.buttonSend = QtWidgets.QPushButton(self.widget_2)
        self.buttonSend.setObjectName("buttonSend")
        self.verticalLayout_2.addWidget(self.buttonSend)
        self.checkBoxHexSend = QtWidgets.QCheckBox(self.widget_2)
        self.checkBoxHexSend.setObjectName("checkBoxHexSend")
        self.verticalLayout_2.addWidget(self.checkBoxHexSend)
        self.gridLayout.addWidget(self.widget_2, 2, 0, 1, 1)
        self.plainTextEdit = QtWidgets.QPlainTextEdit(FormSerialPort)
        self.plainTextEdit.setObjectName("plainTextEdit")
        self.gridLayout.addWidget(self.plainTextEdit, 2, 1, 1, 1)
        self.gridLayout.setColumnStretch(1, 2)
        self.gridLayout.setRowStretch(0, 3)

        self.retranslateUi(FormSerialPort)
        self.comboBoxBaud.setCurrentIndex(3)
        self.comboBoxData.setCurrentIndex(3)
        self.pushButton_2.clicked.connect(self.textBrowser.clear)
        QtCore.QMetaObject.connectSlotsByName(FormSerialPort)

    def retranslateUi(self, FormSerialPort):
        _translate = QtCore.QCoreApplication.translate
        FormSerialPort.setWindowTitle(_translate("FormSerialPort", "串口调试小助手"))
        self.label.setText(_translate("FormSerialPort", "端  口"))
        self.label_2.setText(_translate("FormSerialPort", "波特率"))
        self.comboBoxBaud.setItemText(0, _translate("FormSerialPort", "1200"))
        self.comboBoxBaud.setItemText(1, _translate("FormSerialPort", "2400"))
        self.comboBoxBaud.setItemText(2, _translate("FormSerialPort", "4800"))
        self.comboBoxBaud.setItemText(3, _translate("FormSerialPort", "9600"))
        self.comboBoxBaud.setItemText(4, _translate("FormSerialPort", "19200"))
        self.comboBoxBaud.setItemText(5, _translate("FormSerialPort", "38400"))
        self.comboBoxBaud.setItemText(6, _translate("FormSerialPort", "57600"))
        self.comboBoxBaud.setItemText(7, _translate("FormSerialPort", "115200"))
        self.label_3.setText(_translate("FormSerialPort", "校验位"))
        self.comboBoxParity.setItemText(0, _translate("FormSerialPort", "No"))
        self.comboBoxParity.setItemText(1, _translate("FormSerialPort", "Even"))
        self.comboBoxParity.setItemText(2, _translate("FormSerialPort", "Odd"))
        self.comboBoxParity.setItemText(3, _translate("FormSerialPort", "Space"))
        self.comboBoxParity.setItemText(4, _translate("FormSerialPort", "Mark"))
        self.comboBoxParity.setItemText(5, _translate("FormSerialPort", "Unknown"))
        self.label_4.setText(_translate("FormSerialPort", "数据位"))
        self.comboBoxData.setItemText(0, _translate("FormSerialPort", "5"))
        self.comboBoxData.setItemText(1, _translate("FormSerialPort", "6"))
        self.comboBoxData.setItemText(2, _translate("FormSerialPort", "7"))
        self.comboBoxData.setItemText(3, _translate("FormSerialPort", "8"))
        self.label_5.setText(_translate("FormSerialPort", "停止位"))
        self.comboBoxStop.setItemText(0, _translate("FormSerialPort", "OneStop"))
        self.comboBoxStop.setItemText(1, _translate("FormSerialPort", "OneAndHalfStop"))
        self.comboBoxStop.setItemText(2, _translate("FormSerialPort", "TwoStop"))
        self.comboBoxStop.setItemText(3, _translate("FormSerialPort", "UnknownStopBits"))
        self.buttonConnect.setText(_translate("FormSerialPort", "打开串口"))
        self.labelStatus.setText(_translate("FormSerialPort", "      "))
        self.pushButton_2.setText(_translate("FormSerialPort", "清空接收区"))
        self.checkBoxHexView.setText(_translate("FormSerialPort", "十六进制显示"))
        self.buttonSend.setText(_translate("FormSerialPort", "手动发送"))
        self.checkBoxHexSend.setText(_translate("FormSerialPort", "十六进制发送"))


if __name__ == "__main__":
    import sys
    app = QtWidgets.QApplication(sys.argv)
    FormSerialPort = QtWidgets.QWidget()
    ui = Ui_FormSerialPort()
    ui.setupUi(FormSerialPort)
    FormSerialPort.show()
    sys.exit(app.exec_())



```

## Useful links

- Learn PyQt: https://pythonbasics.org/pyqt-hello-world/
- Install PyQt: https://pythonbasics.org/install-pyqt/