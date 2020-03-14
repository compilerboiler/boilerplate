---
tags: ["python"]
date: 2020-02-14
title: read csv in python
---
A csv file is a file in which data is separated by a delimiter (often a comma). Many office programs can store data in a csv format (<a href="https://sites.google.com/a/temple.edu/googleapps1/tip-of-the-day/april28-exportagooglespreadsheetintovariousformats">Google Sheet</a>, <a href="https://answers.microsoft.com/en-us/msoffice/forum/all/how-to-save-excel-file-in-csv-with-comma-delimited/7ee047dc-8f37-42d4-9be9-954fcf5de2da">Microsoft Excel</a> etc).

The file format is just that simple: a bunch of data which is divided using a delimiter (sometimes called the separator). Example CSV file data:

```
1/2/2020,5,5,8,white
1/3/2020,3,5,2,blue
1/4/2020,2,9,1,green
```

CSV only stores data (values), not formatting. So if you save as a csv file, you lose all formatting you had before. Now for Python programs, formatting is totally irrelevant.

![csv file loses formatting](https://dev-to-uploads.s3.amazonaws.com/i/n7ju06igw72k58xsqvfs.png)

## read csv

In Python, you can read a csv file. You can then use its data in your program. There are several ways to read a csv file with Python.

* without any module 
* read with csv module
* read with <a href="https://pythonspot.com/pandas-read-csv/">pandas module</a> module

To read a csv without any module, <a href="https://pythonbasics.org/read-file/">read the file</a> first and then use the <a href="https://pythonbasics.org/split/">split</a> function with delimiter to extract values (*txt.split(",")*).


If you deal with data a lot, I recommend to use the <a href="https://pandas.pydata.org/">Pandas module</a>. Pandas is a fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language. 

You can use pandas to read other data sources too (like <a href="https://pythonspot.com/read-excel-with-pandas/">excel</a>).  A good course for Pandas is <a href="https://gumroad.com/l/KmxqY">data analysis with pandas</a>

## csv module

With the csv module you can read a csv file like this. First import the csv module. Then read the file, define the delimiter and iterate row by row.

```python
import csv

with open('example.csv') as csvfile:
    csvfile = csv.reader(csvfile, delimiter=',')
    for row in csvfile:
        print(row)
```

Every row is a list of values in the csv file.

```bash
$ python3 example.py 
['1/2/2020', '5', '5', '8', 'white']
['1/3/2020', '3', '5', '2', 'blue']
['1/4/2020', '2', '9', '1', 'green']
```

**Related links:**
* <a href="https://pythonspot.com/files-spreadsheets-csv/">More csv module examples</a>
* <a href="https://pythonbasics.org/">Learn Python</a>



