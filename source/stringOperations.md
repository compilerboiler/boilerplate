---
title: stringOperations (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'stringOperations'


## stringOperations

Python beginners example: stringOperations

```python
# This example shows you string operations

name = 'Kalpak'
print('My name is ' + name) # I have given space after is notice

age = 14
print('My age is ', age) # comma seprates two different things you want to print

print('This isn\'t going away too soon.') # that \ is called as an escape character
# the \ is used to use same quote in a string

print('I love newlines \n') # \n prints new line after string or according to its position

print('\t I love tabs') # \t adds a tab according to its position

multiple = 'Iron Man'
print(multiple * 5) # this will print(string 5 times)

# string methods in built
country = 'Norway'
print(country.upper()) # prints all letters in upper case
print(country.lower()) # prints all letters in lower case
print(country.title()) # converts into title

# string formatting
print('%s %s %s'%('I' , 'am' , 'cool'))

expression = 'I love'
movie = 'Captain America 3'
print('%s %s'%(expression , movie))

# type conversion
addition = 12343 + 3349
print('The answer is ' + str(addition)) # str() method converts non-string into string


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
- Another Python site: https://pythonprogramminglanguage.com
