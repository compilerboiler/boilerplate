---
title: SumOfSquares (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'SumOfSquares'

Functions in program: 
* def sumOfSquares(n):

## SumOfSquares

Python beginners example: SumOfSquares

```python
# Program to print(Sum of Squares of first 'n' natural numbers)

def sumOfSquares(n):
    sum = 0
    for x in range(1,n+1):
        sum = sum + pow(x,2)
    return sum

n = int(input("Enter value of n for generating sum of sqaures:"))
print("Sum of Squares of first",n ,"numbers is : ", sumOfSquares(n))

```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
- Another Python site: https://pythonprogramminglanguage.com
