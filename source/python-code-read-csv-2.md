---
title: python code read csv 2 (snippet)
date: 2020-02-15
tags: ["python"]
---
Python example 'python code read csv 2'


Modules used in program: 
* `import csv`

## python code read csv 2

Python code example: python code read csv 2

```python

# CSV reader solution
import csv
csv_mapping_list = []
with open("/path/to/data.csv") as my_data: 
  csv_reader = csv.reader(my_data, delimiter=",") 
  line_count = 0 
  for line in csv_reader: 
    if line_count == 0: 
      header = line 
    else: 
      row_dict = {key: value for key, value in zip(header, line)} 
      csv_mapping_list.append(row_dict) 
    line_count += 1


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org

More Python: https://pythonprogramminglanguage.com
