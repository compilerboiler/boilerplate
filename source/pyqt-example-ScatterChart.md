---
title: pyqt example ScatterChart (snippet)
date: 2020-02-10
tags: ["python"]
---
Python pyqt (gui) example 'ScatterChart'


Modules used in program: 
* `import random`

## ScatterChart

Python pyqt example: ScatterChart

```python
#!/usr/bin/env python
# -*- coding: utf-8 -*-

"""
Created on 2019/10/2
@author: Irony
@site: https://pyqt5.com , https://github.com/892768447
@email: 892768447@qq.com
@file: ScatterChart
@description: 散点图表
"""
import random

from PyQt5.QtChart import QChartView, QChart, QScatterSeries
from PyQt5.QtCore import QPointF
from PyQt5.QtGui import QPainter


class Window(QChartView):

    def __init__(self, *args, **kwargs):
        super(Window, self).__init__(*args, **kwargs)
        self.resize(400, 300)
        # 抗锯齿
        self.setRenderHint(QPainter.Antialiasing)
        # 生成模拟数据
        self.m_dataTable = self.generateRandomData(3, 10, 7)

        # 图表
        chart = QChart()
        self.setChart(chart)
        # 设置标题
        chart.setTitle('Scatter chart')
        # 添加Series
        self.getSeries(chart)
        # 创建默认xy轴
        chart.createDefaultAxes()
        chart.legend().setVisible(False)

    def getSeries(self, chart):
        for i, data_list in enumerate(self.m_dataTable):
            series = QScatterSeries(chart)
            for value, _ in data_list:
                series.append(value)

            series.setName('Series ' + str(i))
            chart.addSeries(series)

    def generateRandomData(self, listCount, valueMax, valueCount):
        # 生成模拟随机数据
        random.seed()

        dataTable = []

        for i in range(listCount):
            dataList = []
            yValue = 0.0
            f_valueCount = float(valueCount)

            for j in range(valueCount):
                yValue += random.uniform(0, valueMax) / f_valueCount
                value = QPointF(j + random.random() * valueMax / f_valueCount, yValue)
                label = 'Slice ' + str(i) + ':' + str(j)
                dataList.append((value, label))

            dataTable.append(dataList)

        return dataTable


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
