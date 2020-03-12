---
title: python code python-code-sort-list-of-dictionaries (snippet)
date: 2019-02-15
tags: ["python"]
---
Python example 'python code python-code-sort-list-of-dictionaries'


## python code python-code-sort-list-of-dictionaries

Python code example: python code python-code-sort-list-of-dictionaries

```python
csv_mapping_list = [
  { "Name": "Jeremy", "Age": 25, "Favorite Color": "Blue" }, 
  { "Name": "Ally", "Age": 41, "Favorite Color": "Magenta" }, 
  { "Name": "Jasmine", "Age": 29, "Favorite Color": "Aqua" }
]

# Custom sorting
size = len(csv_mapping_list)
for i in range(size): 
  min_index = i 
  for j in range(i + 1, size): 
    if csv_mapping_list[min_index]["Age"] > csv_mapping_list[j]["Age"]: 
      min_index = j 
      csv_mapping_list[i], csv_mapping_list[min_index] = csv_mapping_list[min_index], csv_mapping_list[i]

# List sorting function
csv_mapping_list.sort(key=lambda item: item.get("Age"))

# List sorting using itemgetter
from operator import itemgetter
f = itemgetter('Name')
csv_mapping_list.sort(key=f)

# Iterable sorted function
csv_mapping_list = sorted(csv_mapping_list, key=lambda item: item.get("Age"))


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
More Python: https://pythonprogramminglanguage.com
