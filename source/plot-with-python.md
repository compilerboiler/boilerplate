---
tags: ["python"]
date: 2020-02-14
title: plot with python
---
Do you want to make beautiful charts with <a href="https://python.org">Python</a>? You can with matplotlib or seaborn.

<a href="https://matplotlib.org/">Matplotlib</a> is a plotting library for the Python programming language. It lets you create charts like a <a href="https://pythonbasics.org/matplotlib-bar-chart/">bar chart</a>, <a href="https://pythonbasics.org/matplotlib-line-chart/">line chart</a> and many other basic charts.

<a href="https://seaborn.pydata.org/">Seaborn</a> is a Python data visualization library based on matplotlib.It provides a high-level interface for drawing attractive and informative statistical graphics.

You should know the <a href="https://pythonbasics.org">basics of Python</a> before trying to make plots.

## Example

So is it complicated to make a plot? It depends. Creating a plot can be as simple as 3 lines of code:

```python
import matplotlib.pyplot as plt

plt.bar([1,2,3,4,5], [10,20,30,40,50])
plt.show()
```

where it's x-values and y-values in the bar parameters. This shows a simple bar chart:

![bar chart](https://dev-to-uploads.s3.amazonaws.com/i/32bqx2dj61ejgbepq5ta.png)

Now that is with matplotlib alone. What about seaborn?

With seaborn you can change the colors, add a grid etc. There are also many other <a href="https://seaborn.pydata.org/examples/index.html">plots</a>. You'll see seaborn looks a lot more modern:

```python
import matplotlib.pyplot as plt
import seaborn as sns

sns.set(style="darkgrid")

plt.bar([1,2,3,4,5], [10,20,30,40,50], color="m")
plt.title("seaborn")
plt.show()
```

![seaborn plot](https://dev-to-uploads.s3.amazonaws.com/i/ll5s80m7xlgujxomqcz2.png)

You can learn both modules, and because seaborn is based on matplotlib, there isn't much of a difference in learning curve.

**Related links:**
* <a href="https://pythonbasics.org/seaborn-distplot/">Seaborn with Python tutorial</a>
* <a href="https://gumroad.com/l/mpdp">Matplotlib Data visualization course</a>
* <a href="https://pythonspot.com/matplotlib-line-chart/">Matplotlib tutorial</a>
