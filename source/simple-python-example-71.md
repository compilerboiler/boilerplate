---
title: simple python-example-71 (snippet)
date: 2020-02-11
tags: ["python"]
---
Python example 'python-example-71'

Functions in program: 
* `def output_stu(stu):`
* `def input_stu(stu):`

## python-example-71

Python example: python-example-71

```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

N = 3
#stu
# num : string
# name : string
# score[4]: list
student = []
for i in range(5):
    student.append(['','',[]])

def input_stu(stu):
    for i in range(N):
        stu[i][0] = raw_input('input student num:\n')
        stu[i][1] = raw_input('input student name:\n')
        for j in range(3):
            stu[i][2].append(int(raw_input('score:\n')))

def output_stu(stu):
    for i in range(N):
        print('%-6s%-10s' % ( stu[i][0],stu[i][1] ))
        for j in range(3):
            print('%-8d' % stu[i][2][j])

if __name__ == '__main__':
    input_stu(student)
    print(student)
    output_stu(student)


```

## Useful links

- Learn Python: https://pythonbasics.org/
- More Python: https://pythonprogramminglanguage.com
