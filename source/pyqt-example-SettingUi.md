---
title: pyqt example SettingUi (snippet)
date: 2020-02-10
tags: ["python"]
---
Python pyqt (gui) example 'SettingUi'


## SettingUi

Python pyqt example: SettingUi

```python
# -*- coding: utf-8 -*-

# Form implementation generated from reading ui file 'setting.ui'
#
# Created by: PyQt5 UI code generator 5.5.1
#
# WARNING! All changes made in this file will be lost!

from PyQt5 import QtCore, QtGui, QtWidgets

class Ui_Setting(object):
    def setupUi(self, Setting):
        Setting.setObjectName("Setting")
        Setting.resize(498, 498)
        self.horizontalLayout = QtWidgets.QHBoxLayout(Setting)
        self.horizontalLayout.setContentsMargins(0, 0, 0, 0)
        self.horizontalLayout.setSpacing(0)
        self.horizontalLayout.setObjectName("horizontalLayout")
        self.listWidget = QtWidgets.QListWidget(Setting)
        self.listWidget.setFrameShape(QtWidgets.QFrame.NoFrame)
        self.listWidget.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
        self.listWidget.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
        self.listWidget.setObjectName("listWidget")
        item = QtWidgets.QListWidgetItem()
        self.listWidget.addItem(item)
        item = QtWidgets.QListWidgetItem()
        self.listWidget.addItem(item)
        item = QtWidgets.QListWidgetItem()
        self.listWidget.addItem(item)
        item = QtWidgets.QListWidgetItem()
        self.listWidget.addItem(item)
        item = QtWidgets.QListWidgetItem()
        self.listWidget.addItem(item)
        item = QtWidgets.QListWidgetItem()
        self.listWidget.addItem(item)
        item = QtWidgets.QListWidgetItem()
        self.listWidget.addItem(item)
        item = QtWidgets.QListWidgetItem()
        self.listWidget.addItem(item)
        item = QtWidgets.QListWidgetItem()
        self.listWidget.addItem(item)
        item = QtWidgets.QListWidgetItem()
        self.listWidget.addItem(item)
        item = QtWidgets.QListWidgetItem()
        self.listWidget.addItem(item)
        item = QtWidgets.QListWidgetItem()
        self.listWidget.addItem(item)
        item = QtWidgets.QListWidgetItem()
        self.listWidget.addItem(item)
        self.horizontalLayout.addWidget(self.listWidget)
        self.scrollArea = QtWidgets.QScrollArea(Setting)
        self.scrollArea.setFrameShape(QtWidgets.QFrame.NoFrame)
        self.scrollArea.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
        self.scrollArea.setWidgetResizable(True)
        self.scrollArea.setObjectName("scrollArea")
        self.scrollAreaWidgetContents = QtWidgets.QWidget()
        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, -810, 460, 1308))
        self.scrollAreaWidgetContents.setObjectName("scrollAreaWidgetContents")
        self.verticalLayout = QtWidgets.QVBoxLayout(self.scrollAreaWidgetContents)
        self.verticalLayout.setContentsMargins(35, 20, 35, 20)
        self.verticalLayout.setSpacing(20)
        self.verticalLayout.setObjectName("verticalLayout")
        self.widget_0 = QtWidgets.QWidget(self.scrollAreaWidgetContents)
        self.widget_0.setObjectName("widget_0")
        self.formLayout = QtWidgets.QFormLayout(self.widget_0)
        self.formLayout.setContentsMargins(0, 0, 0, 0)
        self.formLayout.setObjectName("formLayout")
        self.titleLabel1 = QtWidgets.QLabel(self.widget_0)
        self.titleLabel1.setObjectName("titleLabel1")
        self.formLayout.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.titleLabel1)
        self.CheckBox = QtWidgets.QCheckBox(self.widget_0)
        self.CheckBox.setObjectName("CheckBox")
        self.formLayout.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.CheckBox)
        self.checkBox = QtWidgets.QCheckBox(self.widget_0)
        self.checkBox.setChecked(True)
        self.checkBox.setObjectName("checkBox")
        self.formLayout.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.checkBox)
        self.checkBox_2 = QtWidgets.QCheckBox(self.widget_0)
        self.checkBox_2.setChecked(True)
        self.checkBox_2.setObjectName("checkBox_2")
        self.formLayout.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.checkBox_2)
        self.checkBox_3 = QtWidgets.QCheckBox(self.widget_0)
        self.checkBox_3.setObjectName("checkBox_3")
        self.formLayout.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.checkBox_3)
        self.checkBox_4 = QtWidgets.QCheckBox(self.widget_0)
        self.checkBox_4.setObjectName("checkBox_4")
        self.formLayout.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.checkBox_4)
        self.checkBox_5 = QtWidgets.QCheckBox(self.widget_0)
        self.checkBox_5.setObjectName("checkBox_5")
        self.formLayout.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.checkBox_5)
        self.checkBox_6 = QtWidgets.QCheckBox(self.widget_0)
        self.checkBox_6.setObjectName("checkBox_6")
        self.formLayout.setWidget(6, QtWidgets.QFormLayout.FieldRole, self.checkBox_6)
        self.verticalLayout.addWidget(self.widget_0)
        self.widget_1 = QtWidgets.QWidget(self.scrollAreaWidgetContents)
        self.widget_1.setObjectName("widget_1")
        self.formLayout_8 = QtWidgets.QFormLayout(self.widget_1)
        self.formLayout_8.setContentsMargins(0, 0, 0, 0)
        self.formLayout_8.setObjectName("formLayout_8")
        self.titleLabel2 = QtWidgets.QLabel(self.widget_1)
        self.titleLabel2.setObjectName("titleLabel2")
        self.formLayout_8.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.titleLabel2)
        self.checkBox_26 = QtWidgets.QCheckBox(self.widget_1)
        self.checkBox_26.setObjectName("checkBox_26")
        self.formLayout_8.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.checkBox_26)
        self.checkBox_27 = QtWidgets.QCheckBox(self.widget_1)
        self.checkBox_27.setObjectName("checkBox_27")
        self.formLayout_8.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.checkBox_27)
        self.checkBox_28 = QtWidgets.QCheckBox(self.widget_1)
        self.checkBox_28.setObjectName("checkBox_28")
        self.formLayout_8.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.checkBox_28)
        self.checkBox_29 = QtWidgets.QCheckBox(self.widget_1)
        self.checkBox_29.setObjectName("checkBox_29")
        self.formLayout_8.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.checkBox_29)
        self.label_10 = QtWidgets.QLabel(self.widget_1)
        self.label_10.setObjectName("label_10")
        self.formLayout_8.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.label_10)
        self.right1 = QtWidgets.QRadioButton(self.widget_1)
        self.right1.setObjectName("right1")
        self.formLayout_8.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.right1)
        self.right2 = QtWidgets.QRadioButton(self.widget_1)
        self.right2.setChecked(True)
        self.right2.setObjectName("right2")
        self.formLayout_8.setWidget(6, QtWidgets.QFormLayout.FieldRole, self.right2)
        self.label_11 = QtWidgets.QLabel(self.widget_1)
        self.label_11.setObjectName("label_11")
        self.formLayout_8.setWidget(7, QtWidgets.QFormLayout.FieldRole, self.label_11)
        self.right3 = QtWidgets.QPushButton(self.widget_1)
        self.right3.setObjectName("right3")
        self.formLayout_8.setWidget(8, QtWidgets.QFormLayout.FieldRole, self.right3)
        self.verticalLayout.addWidget(self.widget_1)
        self.widget_2 = QtWidgets.QWidget(self.scrollAreaWidgetContents)
        self.widget_2.setObjectName("widget_2")
        self.formLayout_9 = QtWidgets.QFormLayout(self.widget_2)
        self.formLayout_9.setContentsMargins(0, 0, 0, 0)
        self.formLayout_9.setObjectName("formLayout_9")
        self.titleLabel3 = QtWidgets.QLabel(self.widget_2)
        self.titleLabel3.setObjectName("titleLabel3")
        self.formLayout_9.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.titleLabel3)
        self.horizontalLayout_2 = QtWidgets.QHBoxLayout()
        self.horizontalLayout_2.setObjectName("horizontalLayout_2")
        self.label_13 = QtWidgets.QLabel(self.widget_2)
        self.label_13.setObjectName("label_13")
        self.horizontalLayout_2.addWidget(self.label_13)
        self.comboBox = QtWidgets.QComboBox(self.widget_2)
        self.comboBox.setObjectName("comboBox")
        self.comboBox.addItem("")
        self.comboBox.addItem("")
        self.comboBox.addItem("")
        self.comboBox.addItem("")
        self.comboBox.addItem("")
        self.comboBox.addItem("")
        self.horizontalLayout_2.addWidget(self.comboBox)
        spacerItem = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
        self.horizontalLayout_2.addItem(spacerItem)
        self.formLayout_9.setLayout(0, QtWidgets.QFormLayout.FieldRole, self.horizontalLayout_2)
        self.checkBox_30 = QtWidgets.QCheckBox(self.widget_2)
        self.checkBox_30.setObjectName("checkBox_30")
        self.formLayout_9.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.checkBox_30)
        self.right4 = QtWidgets.QLabel(self.widget_2)
        self.right4.setObjectName("right4")
        self.formLayout_9.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.right4)
        self.checkBox_31 = QtWidgets.QCheckBox(self.widget_2)
        self.checkBox_31.setObjectName("checkBox_31")
        self.formLayout_9.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.checkBox_31)
        self.horizontalLayout_3 = QtWidgets.QHBoxLayout()
        self.horizontalLayout_3.setObjectName("horizontalLayout_3")
        self.pushButton_5 = QtWidgets.QPushButton(self.widget_2)
        self.pushButton_5.setObjectName("pushButton_5")
        self.horizontalLayout_3.addWidget(self.pushButton_5)
        self.pushButton_4 = QtWidgets.QPushButton(self.widget_2)
        self.pushButton_4.setObjectName("pushButton_4")
        self.horizontalLayout_3.addWidget(self.pushButton_4)
        spacerItem1 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
        self.horizontalLayout_3.addItem(spacerItem1)
        self.formLayout_9.setLayout(4, QtWidgets.QFormLayout.FieldRole, self.horizontalLayout_3)
        self.verticalLayout.addWidget(self.widget_2)
        self.widget_3 = QtWidgets.QWidget(self.scrollAreaWidgetContents)
        self.widget_3.setObjectName("widget_3")
        self.formLayout_2 = QtWidgets.QFormLayout(self.widget_3)
        self.formLayout_2.setContentsMargins(0, 0, 0, 0)
        self.formLayout_2.setObjectName("formLayout_2")
        self.titleLabel4 = QtWidgets.QLabel(self.widget_3)
        self.titleLabel4.setObjectName("titleLabel4")
        self.formLayout_2.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.titleLabel4)
        self.CheckBox_2 = QtWidgets.QCheckBox(self.widget_3)
        self.CheckBox_2.setChecked(True)
        self.CheckBox_2.setObjectName("CheckBox_2")
        self.formLayout_2.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.CheckBox_2)
        self.checkBox_7 = QtWidgets.QCheckBox(self.widget_3)
        self.checkBox_7.setObjectName("checkBox_7")
        self.formLayout_2.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.checkBox_7)
        self.checkBox_8 = QtWidgets.QCheckBox(self.widget_3)
        self.checkBox_8.setObjectName("checkBox_8")
        self.formLayout_2.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.checkBox_8)
        self.checkBox_9 = QtWidgets.QCheckBox(self.widget_3)
        self.checkBox_9.setChecked(True)
        self.checkBox_9.setObjectName("checkBox_9")
        self.formLayout_2.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.checkBox_9)
        self.checkBox_10 = QtWidgets.QCheckBox(self.widget_3)
        self.checkBox_10.setChecked(True)
        self.checkBox_10.setObjectName("checkBox_10")
        self.formLayout_2.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.checkBox_10)
        self.checkBox_11 = QtWidgets.QCheckBox(self.widget_3)
        self.checkBox_11.setChecked(True)
        self.checkBox_11.setObjectName("checkBox_11")
        self.formLayout_2.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.checkBox_11)
        self.checkBox_12 = QtWidgets.QCheckBox(self.widget_3)
        self.checkBox_12.setChecked(True)
        self.checkBox_12.setObjectName("checkBox_12")
        self.formLayout_2.setWidget(6, QtWidgets.QFormLayout.FieldRole, self.checkBox_12)
        self.checkBox_13 = QtWidgets.QCheckBox(self.widget_3)
        self.checkBox_13.setChecked(True)
        self.checkBox_13.setObjectName("checkBox_13")
        self.formLayout_2.setWidget(7, QtWidgets.QFormLayout.FieldRole, self.checkBox_13)
        self.checkBox_14 = QtWidgets.QCheckBox(self.widget_3)
        self.checkBox_14.setChecked(True)
        self.checkBox_14.setObjectName("checkBox_14")
        self.formLayout_2.setWidget(8, QtWidgets.QFormLayout.FieldRole, self.checkBox_14)
        self.checkBox_15 = QtWidgets.QCheckBox(self.widget_3)
        self.checkBox_15.setChecked(True)
        self.checkBox_15.setObjectName("checkBox_15")
        self.formLayout_2.setWidget(9, QtWidgets.QFormLayout.FieldRole, self.checkBox_15)
        self.verticalLayout.addWidget(self.widget_3)
        self.widget_4 = QtWidgets.QWidget(self.scrollAreaWidgetContents)
        self.widget_4.setObjectName("widget_4")
        self.formLayout_3 = QtWidgets.QFormLayout(self.widget_4)
        self.formLayout_3.setContentsMargins(0, 0, 0, 0)
        self.formLayout_3.setObjectName("formLayout_3")
        self.titleLabel5 = QtWidgets.QLabel(self.widget_4)
        self.titleLabel5.setObjectName("titleLabel5")
        self.formLayout_3.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.titleLabel5)
        self.checkBox_16 = QtWidgets.QCheckBox(self.widget_4)
        self.checkBox_16.setChecked(True)
        self.checkBox_16.setObjectName("checkBox_16")
        self.formLayout_3.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.checkBox_16)
        self.checkBox_17 = QtWidgets.QCheckBox(self.widget_4)
        self.checkBox_17.setChecked(True)
        self.checkBox_17.setObjectName("checkBox_17")
        self.formLayout_3.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.checkBox_17)
        self.checkBox_18 = QtWidgets.QCheckBox(self.widget_4)
        self.checkBox_18.setChecked(True)
        self.checkBox_18.setObjectName("checkBox_18")
        self.formLayout_3.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.checkBox_18)
        self.checkBox_19 = QtWidgets.QCheckBox(self.widget_4)
        self.checkBox_19.setChecked(True)
        self.checkBox_19.setObjectName("checkBox_19")
        self.formLayout_3.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.checkBox_19)
        self.verticalLayout.addWidget(self.widget_4)
        self.widget_5 = QtWidgets.QWidget(self.scrollAreaWidgetContents)
        self.widget_5.setObjectName("widget_5")
        self.formLayout_4 = QtWidgets.QFormLayout(self.widget_5)
        self.formLayout_4.setContentsMargins(0, 0, 0, 0)
        self.formLayout_4.setObjectName("formLayout_4")
        self.titleLabel6 = QtWidgets.QLabel(self.widget_5)
        self.titleLabel6.setObjectName("titleLabel6")
        self.formLayout_4.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.titleLabel6)
        self.checkBox_20 = QtWidgets.QCheckBox(self.widget_5)
        self.checkBox_20.setObjectName("checkBox_20")
        self.formLayout_4.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.checkBox_20)
        self.checkBox_21 = QtWidgets.QCheckBox(self.widget_5)
        self.checkBox_21.setObjectName("checkBox_21")
        self.formLayout_4.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.checkBox_21)
        self.checkBox_22 = QtWidgets.QCheckBox(self.widget_5)
        self.checkBox_22.setObjectName("checkBox_22")
        self.formLayout_4.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.checkBox_22)
        self.checkBox_23 = QtWidgets.QCheckBox(self.widget_5)
        self.checkBox_23.setObjectName("checkBox_23")
        self.formLayout_4.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.checkBox_23)
        self.checkBox_24 = QtWidgets.QCheckBox(self.widget_5)
        self.checkBox_24.setObjectName("checkBox_24")
        self.formLayout_4.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.checkBox_24)
        self.right5 = QtWidgets.QLabel(self.widget_5)
        self.right5.setObjectName("right5")
        self.formLayout_4.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.right5)
        self.label_3 = QtWidgets.QLabel(self.widget_5)
        self.label_3.setObjectName("label_3")
        self.formLayout_4.setWidget(6, QtWidgets.QFormLayout.FieldRole, self.label_3)
        self.label_4 = QtWidgets.QLabel(self.widget_5)
        self.label_4.setObjectName("label_4")
        self.formLayout_4.setWidget(7, QtWidgets.QFormLayout.FieldRole, self.label_4)
        self.radioButton = QtWidgets.QRadioButton(self.widget_5)
        self.radioButton.setObjectName("radioButton")
        self.formLayout_4.setWidget(8, QtWidgets.QFormLayout.FieldRole, self.radioButton)
        self.radioButton_2 = QtWidgets.QRadioButton(self.widget_5)
        self.radioButton_2.setObjectName("radioButton_2")
        self.formLayout_4.setWidget(9, QtWidgets.QFormLayout.FieldRole, self.radioButton_2)
        self.radioButton_3 = QtWidgets.QRadioButton(self.widget_5)
        self.radioButton_3.setChecked(True)
        self.radioButton_3.setObjectName("radioButton_3")
        self.formLayout_4.setWidget(10, QtWidgets.QFormLayout.FieldRole, self.radioButton_3)
        self.formLayout_5 = QtWidgets.QFormLayout()
        self.formLayout_5.setObjectName("formLayout_5")
        self.listWidgetUser = QtWidgets.QListWidget(self.widget_5)
        self.listWidgetUser.setFrameShape(QtWidgets.QFrame.NoFrame)
        self.listWidgetUser.setObjectName("listWidgetUser")
        self.formLayout_5.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.listWidgetUser)
        self.pushButton = QtWidgets.QPushButton(self.widget_5)
        self.pushButton.setObjectName("pushButton")
        self.formLayout_5.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.pushButton)
        self.formLayout_4.setLayout(11, QtWidgets.QFormLayout.FieldRole, self.formLayout_5)
        self.verticalLayout.addWidget(self.widget_5)
        self.widget_6 = QtWidgets.QWidget(self.scrollAreaWidgetContents)
        self.widget_6.setObjectName("widget_6")
        self.formLayout_6 = QtWidgets.QFormLayout(self.widget_6)
        self.formLayout_6.setContentsMargins(0, 0, 0, 0)
        self.formLayout_6.setObjectName("formLayout_6")
        self.titleLabel7 = QtWidgets.QLabel(self.widget_6)
        self.titleLabel7.setObjectName("titleLabel7")
        self.formLayout_6.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.titleLabel7)
        self.label_6 = QtWidgets.QLabel(self.widget_6)
        self.label_6.setObjectName("label_6")
        self.formLayout_6.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.label_6)
        self.pushButton_2 = QtWidgets.QPushButton(self.widget_6)
        self.pushButton_2.setObjectName("pushButton_2")
        self.formLayout_6.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.pushButton_2)
        self.verticalLayout.addWidget(self.widget_6)
        self.widget_7 = QtWidgets.QWidget(self.scrollAreaWidgetContents)
        self.widget_7.setObjectName("widget_7")
        self.formLayout_7 = QtWidgets.QFormLayout(self.widget_7)
        self.formLayout_7.setContentsMargins(0, 0, 0, 0)
        self.formLayout_7.setObjectName("formLayout_7")
        self.titleLabel8 = QtWidgets.QLabel(self.widget_7)
        self.titleLabel8.setObjectName("titleLabel8")
        self.formLayout_7.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.titleLabel8)
        self.checkBox_25 = QtWidgets.QCheckBox(self.widget_7)
        self.checkBox_25.setObjectName("checkBox_25")
        self.formLayout_7.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.checkBox_25)
        self.right6 = QtWidgets.QLabel(self.widget_7)
        self.right6.setObjectName("right6")
        self.formLayout_7.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.right6)
        self.verticalLayout.addWidget(self.widget_7)
        self.scrollArea.setWidget(self.scrollAreaWidgetContents)
        self.horizontalLayout.addWidget(self.scrollArea)

        self.retranslateUi(Setting)
        self.listWidget.setCurrentRow(0)
        QtCore.QMetaObject.connectSlotsByName(Setting)
        Setting.setTabOrder(self.listWidget, self.scrollArea)
        Setting.setTabOrder(self.scrollArea, self.CheckBox)
        Setting.setTabOrder(self.CheckBox, self.checkBox)
        Setting.setTabOrder(self.checkBox, self.checkBox_2)
        Setting.setTabOrder(self.checkBox_2, self.checkBox_3)
        Setting.setTabOrder(self.checkBox_3, self.checkBox_4)
        Setting.setTabOrder(self.checkBox_4, self.checkBox_5)
        Setting.setTabOrder(self.checkBox_5, self.checkBox_6)
        Setting.setTabOrder(self.checkBox_6, self.checkBox_26)
        Setting.setTabOrder(self.checkBox_26, self.checkBox_27)
        Setting.setTabOrder(self.checkBox_27, self.checkBox_28)
        Setting.setTabOrder(self.checkBox_28, self.checkBox_29)
        Setting.setTabOrder(self.checkBox_29, self.right1)
        Setting.setTabOrder(self.right1, self.right2)
        Setting.setTabOrder(self.right2, self.right3)
        Setting.setTabOrder(self.right3, self.comboBox)
        Setting.setTabOrder(self.comboBox, self.checkBox_30)
        Setting.setTabOrder(self.checkBox_30, self.checkBox_31)
        Setting.setTabOrder(self.checkBox_31, self.pushButton_5)
        Setting.setTabOrder(self.pushButton_5, self.pushButton_4)
        Setting.setTabOrder(self.pushButton_4, self.CheckBox_2)
        Setting.setTabOrder(self.CheckBox_2, self.checkBox_7)
        Setting.setTabOrder(self.checkBox_7, self.checkBox_8)
        Setting.setTabOrder(self.checkBox_8, self.checkBox_9)
        Setting.setTabOrder(self.checkBox_9, self.checkBox_10)
        Setting.setTabOrder(self.checkBox_10, self.checkBox_11)
        Setting.setTabOrder(self.checkBox_11, self.checkBox_12)
        Setting.setTabOrder(self.checkBox_12, self.checkBox_13)
        Setting.setTabOrder(self.checkBox_13, self.checkBox_14)
        Setting.setTabOrder(self.checkBox_14, self.checkBox_15)
        Setting.setTabOrder(self.checkBox_15, self.checkBox_16)
        Setting.setTabOrder(self.checkBox_16, self.checkBox_17)
        Setting.setTabOrder(self.checkBox_17, self.checkBox_18)
        Setting.setTabOrder(self.checkBox_18, self.checkBox_19)
        Setting.setTabOrder(self.checkBox_19, self.checkBox_20)
        Setting.setTabOrder(self.checkBox_20, self.checkBox_21)
        Setting.setTabOrder(self.checkBox_21, self.checkBox_22)
        Setting.setTabOrder(self.checkBox_22, self.checkBox_23)
        Setting.setTabOrder(self.checkBox_23, self.checkBox_24)
        Setting.setTabOrder(self.checkBox_24, self.radioButton)
        Setting.setTabOrder(self.radioButton, self.radioButton_2)
        Setting.setTabOrder(self.radioButton_2, self.radioButton_3)
        Setting.setTabOrder(self.radioButton_3, self.listWidgetUser)
        Setting.setTabOrder(self.listWidgetUser, self.pushButton)
        Setting.setTabOrder(self.pushButton, self.pushButton_2)
        Setting.setTabOrder(self.pushButton_2, self.checkBox_25)

    def retranslateUi(self, Setting):
        _translate = QtCore.QCoreApplication.translate
        Setting.setWindowTitle(_translate("Setting", "仿QQ设置面板"))
        __sortingEnabled = self.listWidget.isSortingEnabled()
        self.listWidget.setSortingEnabled(False)
        item = self.listWidget.item(0)
        item.setText(_translate("Setting", "登录"))
        item = self.listWidget.item(1)
        item.setText(_translate("Setting", "主面板"))
        item = self.listWidget.item(2)
        item.setText(_translate("Setting", "状态"))
        item = self.listWidget.item(3)
        item.setText(_translate("Setting", "会话窗口"))
        item = self.listWidget.item(4)
        item.setText(_translate("Setting", "信息展示"))
        item = self.listWidget.item(5)
        item.setText(_translate("Setting", "提醒"))
        item = self.listWidget.item(6)
        item.setText(_translate("Setting", "热键"))
        item = self.listWidget.item(7)
        item.setText(_translate("Setting", "显示"))
        item = self.listWidget.item(8)
        item.setText(_translate("Setting", "声音"))
        item = self.listWidget.item(9)
        item.setText(_translate("Setting", "软件更新"))
        item = self.listWidget.item(10)
        item.setText(_translate("Setting", "文件管理"))
        item = self.listWidget.item(11)
        item.setText(_translate("Setting", "文件共享"))
        item = self.listWidget.item(12)
        item.setText(_translate("Setting", "音视频通话"))
        self.listWidget.setSortingEnabled(__sortingEnabled)
        self.titleLabel1.setText(_translate("Setting", "登录："))
        self.CheckBox.setText(_translate("Setting", "开机时自动启动QQ"))
        self.checkBox.setText(_translate("Setting", "启动QQ时为我自动登录"))
        self.checkBox_2.setText(_translate("Setting", "总是打开登录提示"))
        self.checkBox_3.setText(_translate("Setting", "离线自动启动QQ手机版（仅支持Android）"))
        self.checkBox_4.setText(_translate("Setting", "登录后自动运行QQ宠物"))
        self.checkBox_5.setText(_translate("Setting", "订阅“腾讯视频”，获取量身定制视频资讯"))
        self.checkBox_6.setText(_translate("Setting", "订阅“每日精选”，了解最新商品资讯"))
        self.titleLabel2.setText(_translate("Setting", "主面板："))
        self.checkBox_26.setText(_translate("Setting", "始终保持在其他窗口前端"))
        self.checkBox_27.setText(_translate("Setting", "停靠在桌面边缘时自动隐藏"))
        self.checkBox_28.setText(_translate("Setting", "在任务栏通知区域显示QQ图标"))
        self.checkBox_29.setText(_translate("Setting", "显示天气"))
        self.label_10.setText(_translate("Setting", "关闭主面板时："))
        self.right1.setText(_translate("Setting", "隐藏到任务栏通知区域，不退出程序"))
        self.right2.setText(_translate("Setting", "退出程序"))
        self.label_11.setText(_translate("Setting", "您可以自由定制适合您的面板和功能，使用QQ更有效率"))
        self.right3.setText(_translate("Setting", "界面管理器"))
        self.titleLabel3.setText(_translate("Setting", "状态："))
        self.label_13.setText(_translate("Setting", "登陆后状态为："))
        self.comboBox.setItemText(0, _translate("Setting", "我在线上"))
        self.comboBox.setItemText(1, _translate("Setting", "Q我吧"))
        self.comboBox.setItemText(2, _translate("Setting", "离开"))
        self.comboBox.setItemText(3, _translate("Setting", "忙碌"))
        self.comboBox.setItemText(4, _translate("Setting", "请勿打扰"))
        self.comboBox.setItemText(5, _translate("Setting", "隐身"))
        self.checkBox_30.setText(_translate("Setting", "运行全屏程序时切换至“忙碌“状态””"))
        self.right4.setText(_translate("Setting", "仅在“Q我吧”和“我在线上”状态下生效"))
        self.checkBox_31.setText(_translate("Setting", "离开、忙碌、请勿打扰时自动回复（100字以内）"))
        self.pushButton_5.setText(_translate("Setting", "自动回复设置"))
        self.pushButton_4.setText(_translate("Setting", "快捷回复设置"))
        self.titleLabel4.setText(_translate("Setting", "会话窗口："))
        self.CheckBox_2.setText(_translate("Setting", "使用多彩气泡聊天"))
        self.checkBox_7.setText(_translate("Setting", "不显示广告（会员设置项）"))
        self.checkBox_8.setText(_translate("Setting", "允许来消息时自动弹出窗口"))
        self.checkBox_9.setText(_translate("Setting", "默认使用腾讯视频播放视频文件"))
        self.checkBox_10.setText(_translate("Setting", "允许自动播放魔法表情和超级表情"))
        self.checkBox_11.setText(_translate("Setting", "允许使用QQ秀聊天随动表情"))
        self.checkBox_12.setText(_translate("Setting", "总是显示好友聊天窗口侧边栏"))
        self.checkBox_13.setText(_translate("Setting", "允许接收窗口抖动"))
        self.checkBox_14.setText(_translate("Setting", "显示热词搜索提示"))
        self.checkBox_15.setText(_translate("Setting", "显示历史消息记录"))
        self.titleLabel5.setText(_translate("Setting", "信息展示："))
        self.checkBox_16.setText(_translate("Setting", "在资料卡和迷你信息卡上显示等级图标"))
        self.checkBox_17.setText(_translate("Setting", "在资料卡和迷你卡上显示更新搜索"))
        self.checkBox_18.setText(_translate("Setting", "在聊天窗口内展示好友的更新摘要"))
        self.checkBox_19.setText(_translate("Setting", "在聊天窗口内展示好友互动标识"))
        self.titleLabel6.setText(_translate("Setting", "提醒："))
        self.checkBox_20.setText(_translate("Setting", "会话消息提醒"))
        self.checkBox_21.setText(_translate("Setting", "新邮件提醒"))
        self.checkBox_22.setText(_translate("Setting", "启用QQ看点消息"))
        self.checkBox_23.setText(_translate("Setting", "启用一声问候消息"))
        self.checkBox_24.setText(_translate("Setting", "启用设备连接提醒"))
        self.right5.setText(_translate("Setting", "当插入安卓设备时，提示安装或者更新QQ手机版"))
        self.label_3.setText(_translate("Setting", "<html><head/><body><p>您可以设置是否在屏幕右下角收到来自QQ空间的通知，<a href=\"#\"><span style=\" text-decoration: none; color:#00aaff;\">进入设置</span></a>。</p></body></html>"))
        self.label_4.setText(_translate("Setting", "好友上线提醒"))
        self.radioButton.setText(_translate("Setting", "关闭好友上线提醒"))
        self.radioButton_2.setText(_translate("Setting", "全部好友上线提醒"))
        self.radioButton_3.setText(_translate("Setting", "以下好友上线提醒"))
        self.pushButton.setText(_translate("Setting", "添加"))
        self.titleLabel7.setText(_translate("Setting", "热键："))
        self.label_6.setText(_translate("Setting", "您可以通过点击选择要更改的热键"))
        self.pushButton_2.setText(_translate("Setting", "设置热键"))
        self.titleLabel8.setText(_translate("Setting", "显示："))
        self.checkBox_25.setText(_translate("Setting", "开启QQ适配屏幕DPI"))
        self.right6.setText(_translate("Setting", "关闭选项后QQ将保持默认大小，设置后需要重新登录才能生效"))


if __name__ == "__main__":
    import sys
    app = QtWidgets.QApplication(sys.argv)
    Setting = QtWidgets.QWidget()
    ui = Ui_Setting()
    ui.setupUi(Setting)
    Setting.show()
    sys.exit(app.exec_())



```

## Useful links

- Learn PyQt: https://pythonbasics.org/pyqt-hello-world/
- Install PyQt: https://pythonbasics.org/install-pyqt/