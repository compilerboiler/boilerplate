---
title: python-code-convert-two-lists-to-dict (snippet)
date: 2020-02-15
tags: ["python"]
---
Python example 'python-code-convert-two-lists-to-dict'


## python-code-convert-two-lists-to-dict

Python code example: python-code-convert-two-lists-to-dict

```python
column_names = ['id', 'color', 'style']
column_values = [1, 'red', 'bold']

# Convert two lists into a dictionary with zip and the dict constructor
name_to_value_dict = dict(zip(column_names, column_values))

# Convert two lists into a dictionary with a dictionary comprehension
name_to_value_dict = {key:value for key, value in zip(column_names, column_values)}

# Convert two lists into a dictionary with a loop
name_value_tuples = zip(column_names, column_values) 
name_to_value_dict = {} 
for key, value in name_value_tuples: 
  if key in name_to_value_dict: 
    pass # Insert logic for handling duplicate keys 
  else: 
    name_to_value_dict[key] = value


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org

More Python: https://pythonprogramminglanguage.com
