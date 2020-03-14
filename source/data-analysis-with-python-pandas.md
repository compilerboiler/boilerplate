---
tags: ["python"]
date: 2020-02-16
title: data analysis with python pandas
---
---
tags: ["python"]
date: 2020-02-14
title: data analysis with python pandas
---
<a href="https://pandas.pydata.org/">Pandas</a> is a data analysis module for Python. The module was first developed in 2008 and has become one of the most popular data analysis modules.

You can read all kinds of data into Python with pandas.
This includes <a href="https://pythonprogramminglanguage.com/read-csv/">reading csv data</a> (data from txt), read from a <a href="https://pythonbasics.org/pickle/">pickle</a> object file or even the clipboard.


## Read data with pandas

Pandas is all about data. As programs almost always work with data, it's a good skill to know the pandas module.

If this is your text file (filepath.txt, with tabs)

```
1       2       3
2       3       4
3       4       5
4       5       6
5       6       7
```

Then you can read it into a pandas data frame with the lines:

```python
import pandas as pd
dataset=pd.read_csv("filepath.txt",delimiter="\t")
```

If you have a csv file, you can do

```python
data = pd.read_csv('output_list.txt', sep=",", header=None)
```

You can manually define the columns if your data doesn't have any

```python
data.columns = ["a", "b", "c", "etc."]
```

You can then work with the data frame, selecting on it, filter it etcetera.

Select a column like this:

```python
import pandas as pd
dataset=pd.read_csv("filepath.txt",delimiter="\t")
dataset.columns = ["a", "b", "c"]

print(dataset["b"])
```

This shows all your data from the previously defined text file

```python
➜  ~ python3 zoo.py
0    3
1    4
2    5
3    6
Name: b, dtype: int64
```

**Related links:**
* <a href="https://gumroad.com/l/KmxqY">Python pandas course</a>
* <a href="https://pandas.pydata.org/">Pandas module</a>


