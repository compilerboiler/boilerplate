---
title: simple python-example-67 (snippet)
date: 2020-02-11
tags: ["python"]
---
Python example 'python-example-67'

Functions in program: 
* `def outp(numbers):`
* `def max_min(array):`
* `def inp(numbers):`

## python-example-67

Python example: python-example-67

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

def inp(numbers):
    for i in range(9):
        numbers.append(int(raw_input('input a number:\n')))
    numbers.append(int(raw_input('input a number:\n')))
p = 0
def max_min(array):
    max = min = 0
    for i in range(1,len(array) - 1):
        p = i
        if array[p] > array[max] : max = p
        elif array[p] < array[min] : min = p
    k = max
    l = min
    array[0],array[l] = array[l],array[0]
    array[9],array[k] = array[k],array[9]

def outp(numbers):
    for i  in range(len(numbers)):
        print(numbers[i])

if __name__ == '__main__':
    array = []
    inp(array)
    max_min(array)
    outp(array)


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
