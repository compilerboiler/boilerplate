---
title: python code python-code-read-csv-1 (snippet)
date: 2019-02-15
tags: ["python"]
---
Python example 'python code python-code-read-csv-1'


## python code python-code-read-csv-1

Python code example: python code python-code-read-csv-1

```python
# Brute force solution
csv_mapping_list = []
with open("/path/to/data.csv") as my_data: 
  line_count = 0 
  for line in my_data: 
    row_list = [val.strip() for val in line.split(",")] 
    if line_count == 0: 
      header = row_list 
    else: 
      row_dict = {key: value for key, value in zip(header, row_list)}
      csv_mapping_list.append(row_dict) 
    line_count += 1


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org

More Python: https://pythonprogramminglanguage.com
