---
title: python dictionary (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'python dictionary'. A dictionary is a colelction that contains (key, value) pairs. This example shows how to use a dictionary in Python.


## python dictionary

Python beginners example: python dictionary

```python
#!/usr/bin/python

#A Python dictionary is a collection which contains key value pairs, where the
#key must be an immutable object

# you can also run this in the interpretor

phonebook =  {'joe':'568-564-1109', 'ashish':'657-097-7862'}

print("\nPrinting the phonebook")
print(phonebook)
print("\nPrinting joe's phone number")
phonebook['joe']

print("\nAdding an element to the phonebook")
phonebook['joel'] = '657'
print("\nPrinting the phone number of the newly added contact joel")
print(phonebook['joel'])

print("\nItearating across the phonebook with it's keys")
for k in phonebook.keys():
   print(k, phonebook[k])

print("\nHere's how we remove an element from the dictionary - removing 'joel'")
del(phonebook['joel'])

print("\nIterating across the phonebook with key and value")
for k, v in phonebook.items():
   print(k, v)




```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
