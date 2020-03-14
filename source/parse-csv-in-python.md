---
date: 2020-02-16
title: parse csv in python
---
A CSV (Comma Separated Values) file is a plain text file where each value is separated by a comma. 

Excel can open CSV Files. This is really cool because it means you can output your data into csv from Python and then open it in Excel.

In this article you will learn how to read a CSV file in Python.

Before playing with csv data, you should <a href="https://gumroad.com/l/dcsp">learn Python</a>

## Introduction

Each line of the CSV file is called a record, every record has values that are separated by commas. 

It is separated by a *delimiter*, the default delimiter is the comma. You can choose to use another delimiter such as a semicolon (;) or a pipe (|).

Shown below is the structure of a regular CSV File.

    1,Alice,Cook,32
    2,Bob,Doorman,34
    3,Chris,Electrician,24
    4,Dave,Fieldworker,44

Copy the data and save it as `example.csv`

## Why CSV?

CSV format is a simply plain-text file. That means you can open it with any text editor, but also that it can be opened by any software application.

You can import a csv into a spreadsheet or database storage without any problems. It's data-interchangeable.

Any programming language that can work with files and strings, can work with csv file data. 

## CSV module

You don't need to write parsing code yourself, as every so often, Python has a module available.

The module we'll talk about is the `csv` module. It is already installed, because it's part of the Python standard library.

You can <a href="https://pythonspot.com/reading-csv-files-in-python/">read csv files</a> with the `csv` module, but also write them.

To load the module type:

```python
import csv
```

Then create your program (read.py)

```python
import csv

# Open the csv file in read mode 'r'                                                                                                                                              
with open('example.csv','r') as f:
    # read the file                                                                                                                                                               
    csvReader = csv.reader(f)

    # output every line in a loop                                                                                                                                                 
    for line in csvReader:
        print(line)
```

If you run the program you'll see:

    ➜  ~ python3 read.py 
    ['1', 'Alice', 'Cook', '32']
    ['2', 'Bob', 'Doorman', '34']
    ['3', 'Chris', 'Electrician', '24']
    ['4', 'Dave', 'Fieldworker', '44']
    ➜  ~ 

Successfully parsed!


**Related links:**
* <a href="https://docs.python.org/3.8/library/csv.html">Pythons csv module documentation</a>
* <a href="https://pythonprogramminglanguage.com/read-csv/">Read CSV with Python Pandas</a>

