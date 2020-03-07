---
title: test of divisibility (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'testofdivisibility'

Functions in program: 
* `def testDivisibility():`

## testofdivisibility

Python beginners example: testofdivisibility

```python
# pre code
def testDivisibility():
    print(" ")
    toTest = int(raw_input("Enter number of which you want to test Divisibility : "))
    print(" ")
    test = int(raw_input("Enter number by which you want to test : "))
    if toTest % test == 0 :
        print("-------------Answer---------------- ")
        print(str(toTest) + " is divisible by " + str(test))
    else :
        print(str(toTest) + " is not divisible " + str(test))

print(" ")
print("--------------------Start-------------------")
user = raw_input("Start or End : ")

if user.strip() == "Start" :
        print(testDivisibility())
        print(" ")        
# MAIN code
while True:
        get = raw_input("Start again or End : ")
        if get.strip() == "Start again":
            print("---------------Start Again----------------")
            print(" ")
            continue
        elif get.strip() == "End" :
            print(" ")
            print("------------------Program Ended--------------")
            print(" ")
            break
        else :
            break

    elif user.strip() == "End" :
        print(" ")
        print("------------Program Ended-----------")
        print(" ")
        break

    else :
        print(" ")
        print("Invalid Input. Try again")
        continue


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
