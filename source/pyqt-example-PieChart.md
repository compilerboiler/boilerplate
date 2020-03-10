---
title: pyqt example PieChart (snippet)
date: 2020-02-10
tags: ["python"]
---
Python pyqt (gui) example 'PieChart'


## PieChart

Python pyqt example: PieChart

```python
#!/usr/bin/env python
# -*- coding: utf-8 -*-

"""
Created on 2019/10/2
@author: Irony
@site: https://pyqt5.com , https://github.com/892768447
@email: 892768447@qq.com
@file: PieChart
@description: 饼状图表
"""
from PyQt5.QtChart import QChartView, QChart, QPieSeries
from PyQt5.QtGui import QPainter, QColor


class Window(QChartView):

    def __init__(self, *args, **kwargs):
        super(Window, self).__init__(*args, **kwargs)
        self.resize(400, 300)
        # 抗锯齿
        self.setRenderHint(QPainter.Antialiasing)

        # 图表
        chart = QChart()
        self.setChart(chart)
        # 设置标题
        chart.setTitle('Simple piechart example')
        # 添加Series
        chart.addSeries(self.getSeries())

    def getSeries(self):
        series = QPieSeries()
        slice0 = series.append('10%', 1)
        series.append('20%', 2)
        series.append('70%', 7)
        # 显示label文字
        series.setLabelsVisible()
        series.setPieSize(0.5)
        # 使第一块突出显示
        slice0.setLabelVisible()
        slice0.setExploded()
        # 设置第一块颜色
        slice0.setColor(QColor(255, 0, 0, 100))
        return series


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