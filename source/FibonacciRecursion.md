---
title: FibonacciRecursion (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'FibonacciRecursion'

Functions in program: 
* def fibo(n):

## FibonacciRecursion

Python beginners example: FibonacciRecursion

```python
# Program to Print Fibonacci Series using Recursion

# Recursive function to generate Fibonacci series 
def fibo(n):
    if n<=1:
        return 1
    else:
        return fibo(n-1) + fibo(n-2)
    
noOfTerms = int(input("Enter the number of terms:"))

print("Fibonacci Series:")
for x in range(0,noOfTerms):
    print(fibo(x))

```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
- Another Python site: https://pythonprogramminglanguage.com
