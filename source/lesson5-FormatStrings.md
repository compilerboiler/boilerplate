---
title: lesson5-FormatStrings (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'lesson5-FormatStrings'


## lesson5-FormatStrings

Python beginners example: lesson5-FormatStrings

```python
# The printing of our variables in the last few lessons has not been very
# convenient. Let's learn how to print(variables of any type inline.)

# First I'll set up some variables that we'll use throughout the program.
name = "Vivian"           # string
luckyNumber = 5             #
height = 175.9              
favoriteAnimal = "platypus" 

# We learned in lesson one how to concatenate strings for printing.
output = "My name is " + name
print(output)

# But it isn't possible to combine a string with an int the same way.
# Uncomment lines 16 - 17 to see the problem.
#output = "My lucky number is " + luckynumber
#print(output)

# One solution is to manually cast the number to a string like this.
output = "My lucky number is " + str(luckyNumber)
print(output)

# A better way is to use a format string.
output = "My lucky number is {}.".format(luckyNumber)
print(output)

# The syntax is specific, so note a few things:
#  - The curly braces {} go inside the string and act as blanks to fill.
#  - The .format() method goes immediately after the string.
#  - The .format() method takes one argument for each {} in the string.


# Here is a more complex example. Note that the formatting can happen separately
# from setting up the format string.
output = "My name is {}. I am {}cm tall, and I like the {}."
output = output.format(name, height, favoriteAnimal)
print(output)



# ----------- Exercises Below -----------------

# 1. On line 5 I've indicated that the type of name is a string by making a
#    comment. Do likewise for lines 6 - 8.

# 2. The formatting and printing can all be done on one line. Although this
#    isn't always the best choice, in simple cases, it is nice to be concise.
#    Add line 39 to make the program print("Orndorff's lucky number is 5.")
#    Be sure to use a format string.

# 3. Modify lines 6 - 8 so that it asks the user for the values instead of
#    having them "hard-coded". Remember, not all the data is the same type.



```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
