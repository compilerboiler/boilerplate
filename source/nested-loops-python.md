---
date: 2020-02-16
title: nested loops python
---
[Python](https://python.org) language allows loop embedded inside another. A loop repeats one or more lines of code. 

In programming loops are usually [for loops](https://pythonbasics.org/for-loops/). If a loop is inside another loop, this is called a nested loop. You can make nested loops with a [while loop](https://pythonprogramminglanguage.com/while-loop/).

Python for loop nested syntax:

```python
    for iterating_var in sequence:
       for iterating_var in sequence:
          statements (s)
       statements (s)
```

Python while loop nested syntax:

```
    while expression:
       while expression:
          statement (s)
       statement (s)
```

You can be embedded in a loop inside the loop body, such as a while loop  embedded in the for loop, and vice versa, you can embed in a for loop in a while loop.

## Example

The following example uses a prime number between 2 and 100 nested loop output:

```python
i = 2
while (i <100):
   j = 2
   while (j <= (i / j)):
      if not (i% j): break
      j = j + 1
   if (j > (i / j)):
      print(i, "is a prime number.")
   i = i + 1

print("Bye bye!")
```

Examples of the above output:

```
    2 is a prime number
    3 is a prime number
    5 is a prime number
    7 is a prime number
    11 is a prime number
    13 is a prime number
    17 is a prime number
    19 is a prime number
    23 is a prime number
    29 is a prime number
    31 is a prime number
    37 is a prime number
    41 is a prime number
    43 is a prime number
    47 is a prime number
    53 is a prime number
    59 is a prime number
    61 is a prime number
    67 is a prime number
    71 is a prime number
    73 is a prime number
    79 is a prime number
    83 is a prime number
    89 is a prime number
    97 is a prime number
    Bye bye!
```

## More examples

Example: using nested loop to obtain a prime number less than 100

```python
num = [];
i = 2
for i in range (2,100):
   j = 2
   for j in range(2, i):
      if (i% j == 0):
         break
   else:
      num.append(i)
print (num)
```

Example 2: nested loop to draw a pyramid

```python
i = 1
# J = 1                                                                                                                                                                                  
while i <= 9:
   if i <= 5:
      print ("*" * i)

   elif i <= 9:
      j = i-2 * (i-5)
      print ("*" * j)
   i += 1
else:
   print ("")
```
This outputs a sideways pyramid:

```
*
**
***
****
*****
****
***
**
*
```

