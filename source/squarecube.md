---
title: squarecube (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'squarecube'

Functions in program: 
* def square():

## squarecube

Python beginners example: squarecube

```python
# pre code

def square():
    print(" ")
    makeUse = raw_input("Square or Cube : ")
    if makeUse.strip() == "Square":
        print(" ")
        user = int(raw_input("Enter number to get square : "))
        square = user ** 2
        print(" ")
        print("Square of the number " + str(user) + " is " + str(square))
    elif makeUse.strip() == "Cube":
        print(" ")
        userAgain = int(raw_input("Enter number to get square : "))
        cube = userAgain ** 3
        print(" ")
        print("Cube of the number " + str(userAgain) + " is " + str(cube))

# main code

while True:
    print("Hello,")
    print(" ")
    startOrEnd = raw_input("Start or End : ")
    print(" ")
    if startOrEnd.strip() == "Start":
        print(square())
    elif startOrEnd.strip() == "End":
        print(" ")
        print(" ")
        print("Program Ended......")
        break
    else :
        print(" ")
        print("Try Again")
        continue
    startagain = ("Start again or End : ")
    print(" ")
    if startagain.strip() == "Start again":
        print(" ")
        print("Starting again.....")
        continue
    elif startagain == "End":
        print(" ")
        print(" ")
        break
    else :
        print(" ")
        print("Try Again")
        continue


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
- Another Python site: https://pythonprogramminglanguage.com
